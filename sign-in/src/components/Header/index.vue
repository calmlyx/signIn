<template>
    <mt-header fixed title="打卡APP" class="header"></mt-header>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>
    @font-face {
        font-family: 'font1';
        src: url('../../common/fonts/font1.ttf');
    }

    .header {
        font-size: 30px;
        font-family: font1;
    }
</style>