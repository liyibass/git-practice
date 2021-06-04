<template>
    <div class="card__container">
        <div class="card__title">
            <div class="title__name">
                <h3>{{ contact.name }} / {{ contact.job }}</h3>
                <a :href="'mailto:'+contact.email">
                    <img src="../static/mail.svg" width="20px">
                </a>
            </div>
            <div>
                <button>編輯</button>
                <button>刪除</button>
            </div>
        </div>
        <div class="card__content">
            <span class="attribute" v-for="characteristic of contact.characteristic" :key="characteristic">
                # {{ characteristic }}
            </span>
        </div>
    </div>
</template>

<script>
export default {
  props: {
    contact: Object
  }
}
</script>

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
        background-color: #426085;
        padding: 5px 10px;
        font-size: 12px;
        border-radius: 10px;
        color: white;
        margin-right: 10px;
    }
    .title__name {
        display: flex;
        align-items: flex-end;
    }
    img {
        margin-left: 10px;
    }
</style>
