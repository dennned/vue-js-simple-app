<template>
    <li>
        <span v-bind:class="{done: todo.completed}">
            <input type="checkbox" />
            <strong>{{todo.id}}</strong>
            {{todo.title}}
        </span>
        <button class="btn">&times;</button>
    </li>
</template>

<script>
    export default {
        props: {
            todo: {
                type:Object,
                required: true
            }
        }
    }
</script>

<style scoped>
    li {
        border :1px solid #ccc;
        display: flex;
        justify-content: space-between;
        margin: .5rem 2rem;
        padding: 0 0 1rem 0;
    }
    .btn {
        background: red;
        color: #fff;
        border-radius: 50%;
        font-weight: bold;
    }
    input {
        margin-right:1rem;
    }
    .done {
        text-decoration: line-through;
    }
</style>
