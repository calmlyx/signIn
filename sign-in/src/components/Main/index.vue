<template>
    <div class="page-tabbar">
        <div class="page-wrap" style="margin: 0;padding: 0;">
            <div>
                <mt-cell class="page-part" :value="selected" />
            </div>
            <!-- tabcontainer -->
            <mt-tab-container class="page-tabbar-container" v-model="selected">
                <mt-tab-container-item id="首页">
                    <Home></Home>
                </mt-tab-container-item>
                <mt-tab-container-item id="知识聚合">
                    <Knowledge></Knowledge>
                </mt-tab-container-item>
                <mt-tab-container-item id="关于我们">
                    <Aboutus></Aboutus>
                </mt-tab-container-item>
                <mt-tab-container-item id="个人中心">
                     <Me></Me>
                </mt-tab-container-item>
            </mt-tab-container>
        </div>
        <mt-tabbar v-model="selected" fixed>
            <mt-tab-item id="首页">
                <img slot="icon" src="../../assets/footer3.png">
                首页
            </mt-tab-item>
            <mt-tab-item id="知识聚合">
                <img slot="icon" src="../../assets/footer4.png">
                知识聚合
            </mt-tab-item>
            <mt-tab-item id="关于我们">
                <img slot="icon" src="../../assets/footer1.png">
                关于我们
            </mt-tab-item>
            <mt-tab-item id="个人中心">
                <img slot="icon" src="../../assets/Me.png">
                个人中心
            </mt-tab-item>
        </mt-tabbar>
    </div>
</template>

<script>

    import Home from '../Home'
    import Me from '../Me'
    import Knowledge from '../Knowledge'
    import Aboutus from '../Aboutus'   

    export default {
        name: "Main",
        data() {
            return {
                selected: '首页'
            };
        },
        components:{
            Home,
            Me,
            Knowledge,
            Aboutus

        }

    }
</script>

<style scoped>

</style>