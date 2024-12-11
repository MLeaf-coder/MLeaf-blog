<template>
    <div class="blog">
        <div class="avatar">
            <div class="card">
                <div class="avatar-image">
                    <img src="@/assets/img/tx.jpg" alt="Avatar">
                </div>
                <div class="user-info">
                    <div class="user-name">
                        <h1>{{ config.author }}</h1>
                        <hr class="thick-hr">
                    </div>
                    <div class="user-introduction">
                        <p>{{ config.introduce }}</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="blog-post">
            <div class="post-header">
                <div>
                    <div class="post-thumbnail">
                        <img src="@/assets/img/2.jpg" alt="Post Preview">
                    </div>
                </div>
                <div class="post-details">
                    <div class="post-title">
                        <div>
                            <h1>文章测试</h1>
                            <hr class="thick-hr">
                        </div>
                        <div class="post-meta">
                            <div class="meta-item">
                                <CalendarIcon />
                                <p>2023-05-05</p>
                            </div>
                            <div class="meta-item">
                                <BookmarkDoubleIcon />
                                <p>分类</p>
                            </div>
                            <div class="meta-item">
                                <HashtagIcon />
                                <p>标签</p>
                            </div>
                            <div class="meta-item">
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
import { CalendarIcon, BookmarkDoubleIcon, HashtagIcon } from 'tdesign-icons-vue-next'
import config from '@/config/Config';
</script>

<style scoped>
.post-meta {
    display: flex;
    gap: 10px;
    flex-direction: column;
    margin-top: 20px;

}

.post-meta p {
    font-size: 16px;

}

.post-meta svg {
    width: 30px;
    height: 30px;
    margin-right: 10px;
}

.post-details {
    margin-left: 30px;
    margin-top: 20px;

}

.post-title {
    display: flex;
    flex-direction: column;
}

.meta-item {
    display: flex;
}

.blog {
    display: flex;
    justify-content: center;
    width: 100%;
    background: #fff;
}

.meta {
    display: flex;
    gap: 10px;
}

.title-info {
    display: flex;
    height: 100%;
}

.card-corner {
    height: 100%;
    width: 50%;
}

.title-text {
    margin-left: 30px;
}

.event-note {
    display: flex;
    align-items: center;
    gap: 5px;
}

.event-note p {
    margin: 0;
}

.thick-hr {
    border: none;
    height: 5px;
    background-color: rgb(255, 173, 173);

}

.contact {
    width: 100%;
    font-weight: 700;
}

.info {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 10px;
}

.card {
    width: 290px;
    background-color: var(--background-color);
    display: flex;
    flex-direction: column;
    align-items: center;
    box-shadow: 0 0 4px rgba(194, 194, 194, 0.497);
}

.blog-post {
    box-shadow: 0 0 4px rgba(194, 194, 194, 0.497);
    margin-left: 20px;
}

.post-header {
    width: 1045px;
    height: 400px;
    background-color: var(--background-color);
    display: flex;
    margin-left: 10px;
}

.post-header img {
    width: 300px;
    height: 400px;
    object-fit: cover;
    border-radius: 20px;
}

.avatar-image img {
    margin: 15px;
    width: 260px;
    height: 260px;
    border-radius: 20px;
}
</style>