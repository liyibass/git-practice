<template>
    <div class="card__container">
        <div class="card__title">
            <div class="title__name">
                <h3>我是名字 / 我是職稱</h3>
                <img src="../static/mail.svg" width="20px"/>
            </div>
            <div>
                <button>編輯</button>
                <button>刪除</button>
            </div>
        </div>
        <div class="card__content">
            <span class="attribute">#我是屬性</span>
            <span class="attribute">#我是屬性</span>
        </div>
    </div>
</template>

<style scoped>
    button {
        padding: 5px 5px;
        background-color: white;
        color: #35495e;
    }
    .card__container {
        margin-top: 20px;
        padding: 20px;
        box-shadow:1px 1px 3px 1px #3f567234;
        word-break: break-all
    }
    .card__title {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .card__content {
        margin-top: 10px;
    }
    .email {
        margin-top: 10px;
    }
    .attribute {
        background-color: #597fad;
        padding: 5px;
        font-size: 12px;
        border-radius: 10px;
        color: white;
    }
    .title__name {
        display: flex;
    }
    img {
        margin-left: 10px;
    }
</style>
