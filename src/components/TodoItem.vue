<template>
    <li>
        <span v-bind:class="{done: todo.completed}">
            <input type="checkbox"
                   v-on:change="todo.completed = !todo.completed" />
            <strong>{{index + 1}}</strong>
            {{todo.title | uppercase}}
        </span>
        <button class="btn"
            v-on:click="$emit('remove-todo', todo.id)"
        >&times;</button>
    </li>
</template>

<script>
    export default {
        props: {
            todo: {
                type:Object,
                required: true
            },
            index: Number
        },
        filters: {
            uppercase(value) {
                return value.toUpperCase()
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
