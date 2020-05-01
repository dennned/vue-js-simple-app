<template>
    <div class="loadingio-spinner-dual-ring-7by3bo29ola"><div class="ldio-72444xdzd8p">
        <div></div><div><div></div></div>
    </div></div>
</template>

<style>
    @keyframes ldio-72444xdzd8p {
        0% { transform: rotate(0) }
        100% { transform: rotate(360deg) }
    }
    .ldio-72444xdzd8p div { box-sizing: border-box!important }
    .ldio-72444xdzd8p > div {
        position: absolute;
        width: 144px;
        height: 144px;
        top: 28px;
        left: 28px;
        border-radius: 50%;
        border: 16px solid #000;
        border-color: #85a2b6 transparent #85a2b6 transparent;
        animation: ldio-72444xdzd8p 1s linear infinite;
    }
    .ldio-72444xdzd8p > div:nth-child(2) { border-color: transparent }
    .ldio-72444xdzd8p > div:nth-child(2) div {
        position: absolute;
        width: 100%;
        height: 100%;
        transform: rotate(45deg);
    }
    .ldio-72444xdzd8p > div:nth-child(2) div:before, .ldio-72444xdzd8p > div:nth-child(2) div:after {
        content: "";
        display: block;
        position: absolute;
        width: 16px;
        height: 16px;
        top: -16px;
        left: 48px;
        background: #85a2b6;
        border-radius: 50%;
        box-shadow: 0 128px 0 0 #85a2b6;
    }
    .ldio-72444xdzd8p > div:nth-child(2) div:after {
        left: -16px;
        top: 48px;
        box-shadow: 128px 0 0 0 #85a2b6;
    }
    .loadingio-spinner-dual-ring-7by3bo29ola {
        width: 200px;
        height: 200px;
        display: inline-block;
        overflow: hidden;
        background: #f1f2f3;
    }
    .ldio-72444xdzd8p {
        width: 100%;
        height: 100%;
        position: relative;
        transform: translateZ(0) scale(1);
        backface-visibility: hidden;
        transform-origin: 0 0; /* see note above */
    }
    .ldio-72444xdzd8p div { box-sizing: content-box; }
</style>
