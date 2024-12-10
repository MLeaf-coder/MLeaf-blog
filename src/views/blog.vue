<template>
    <div class="blog">
        <div class="avatar">
            <div class="card corner">
                <div class="tx">
                    <img src="@/assets/img/tx.jpg" alt="The">
                </div>
                <div class="info">
                    <div class=" name">
                        <h1>{{ config.author }}</h1>
                        <hr class="thick-hr">
                    </div>
                    <div class="introduce">
                        <p>{{ config.introduce }}</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="blogpost">
            <div class="title corner">
                <div>
                    <div class="img">
                        <img src="@/assets/img/2.jpg" alt="Preview">
                    </div>
                </div>
                <div class="title-info">
                    <div class="title-text">
                        <div>
                            <h1>文章测试</h1>
                            <hr class="thick-hr">
                        </div>
                        <div class="meta">
                            <div class="EventNote">

                                <p>2023-05-05</p>
                            </div>
                            <div class="EventNote">

                                <p>分类</p>
                            </div>
                            <div class="EventNote">

                                <p>标签</p>
                            </div>
                            <div>
                                <p>阅读量</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import config from '@/config/Config';
</script>

<style scoped>
.blog {
    display: flex;
    width: 100%;
    justify-content: center;
    background: #fff;

}

.meta {
    gap: 10px;
}

.title-info {
    display: flex;
    height: 100%;

}

.cardzcorner {
    height: 100%;
    width: 50%;
}

.title-text {
    margin-left: 30px;
}

.EventNote {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 5px;
}

.EventNote p {
    margin: 0;

}

.thick-hr {
    border: none;
    height: 5px;
    background-color: rgb(255, 173, 173);
    margin-top: -15px;
}

.contact {
    width: 100%;
    font-weight: 700;
}

.info {
    display: flex;
    width: auto;
    height: auto;
    flex-direction: column;
    align-items: center;
    margin: 10px;
}

.card {
    width: 290px;
    height: auto;
    background-color: var(--background-color);
    display: flex;
    justify-content: space-around;
    flex-direction: column;
    align-items: center;
    box-shadow: 0 0 4px rgba(194, 194, 194, 0.497);
}

.blogpost {
    box-shadow: 0 0 4px rgba(194, 194, 194, 0.497);
    margin-left: 20px;
}

.title {
    width: 1045px;
    height: 400px;
    background-color: var(--background-color);
    display: flex;
    margin-left: 10px;
}

.title img {
    width: 300px;
    height: 400px;
    object-fit: cover;
    border-radius: 20px;
}

.tx img {
    margin: 15px;
    width: 260px;
    height: 260px;
    border-radius: 20px;
}
</style>