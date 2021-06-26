<template>
    <div class="banner">
        <!-- 顶部导航栏 -->
        <!-- 背景层 -->
        <div class="bg"></div>
        <!-- 个人区 -->
        <div class="presentation">
            <img class="avatar" src="../assets/avatar.jpeg"/> <br>
            <vue-typer :text="title" class="title" eraseStyle="backspace"></vue-typer>
        </div>
    </div>
</template>

<script>
import {VueTyper} from 'vue-typer'

export default {
    name: "Banner",
    components: {
        VueTyper
    },

    data () {
        return {
            title: '梅勒斯的个人主页'
        }
    }
}
</script>

<style>
@font-face{
    font-family: 'custom_ch'; 
    src: url('../assets/font/YanShiYouRanXiaoKai/YanShiYouRanXiaoKai-2.ttf') format('truetype');
}
.banner {
    display: flex;
    width: 100vw;
    height: 100%;
}
.bg {
    width: 100%;
    height: 100%;
    background: url('../assets/background.jpg') no-repeat center center scroll;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    background-size: cover;
    filter: blur(3px);
}
.presentation {
    margin: 20vh auto;
}
.avatar {
    width: 8vw;
    height: 8vw;
    border-radius: 50%;
}
.title {
    font-family: 'custom_ch';
    font-size: 30px;
    margin: 0;
}
</style>
