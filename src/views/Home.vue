<script setup>
import Blog from '@/views/blog.vue';
import config from '@/config/Config';
</script>

<template>
    <div class="root">
        <div class="container">
            <div class="left">
                <img src="@/assets/img/1.png" alt="The">
            </div>
            <div class="side">
                <div class="parcel">
                    <div class="introduce">
                        <h1>{{ config.introduce }}</h1>
                    </div>
                    <div class="content">
                        <p>{{ config.Message }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="main">
        <div class="wave"></div>
        <div class="wave"></div>
        <div class="wave"></div>
    </div>
    <div style="display: flex;justify-content: center;width: 100%;">
        <Blog />
    </div>


</template>

<style scoped>
.root {
    display: flex;
    height: auto;
    width: auto;
    flex-direction: row;
    justify-content: center;
    margin-top: 150px;
}

.container {
    display: flex;
    height: 600px;
    width: 1310px;
}

.side {
    background-color: var(--background-color);
    width: 880px;
    border-radius: 20px;
    box-shadow: 0 0 4px rgb(102, 102, 102);
    padding: 20px;
    box-sizing: border-box;
    font-size: var(--side--font-size);
}


.left img {
    width: 440px;
    object-fit: contain;

}


.main {
    display: flex;
    position: sticky;
    z-index: -1;
    width: 100%;
    overflow: hidden;
    height: 250px;
}

.wave {
    background: rgb(255, 255, 255);
    border-radius: 1000% 1000% 0 0;
    position: absolute;
    width: 200%;
    height: 12em;
    animation: wave 10s -3s linear infinite;
    transform: translate3d(0, 0, 0);
    opacity: 0.8;
    bottom: 0;
    left: 0;
    z-index: -8;
    overflow: hidden;
}

.wave:nth-of-type(2) {
    bottom: -1.25em;
    animation: wave 18s linear reverse infinite;
    opacity: 0.8;
    position: absolute;
    z-index: -9;
    overflow: hidden;
}

.wave:nth-of-type(3) {
    bottom: -2.5em;
    animation: wave 20s -1s reverse infinite;
    opacity: 0.9;
    padding: absolute;
    z-index: -10;
    overflow: hidden;
}

@keyframes wave {
    2% {
        transform: translateX(1);
    }

    25% {
        transform: translateX(-25%);
    }

    50% {
        transform: translateX(-50%);
    }

    75% {
        transform: translateX(-25%);
    }

    100% {
        transform: translateX(1);
    }
}
</style>