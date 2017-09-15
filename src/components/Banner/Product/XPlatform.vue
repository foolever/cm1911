<template>
    <div class="banner-component data-platform" v-show="show">
        <p class="b-title"><span>V</span>irtual Simulation</p>
        <p class="b-title-zh">1+N虚拟仿真实验室</p>
        <div class="b-info">
            <p>
                2017年教育部最新发布的4号文件中指出计划在2017-2020年开展示范性虚拟仿真实验教学项目建设等相关事宜，根据文件解读，构思了基于1+N模式的虚拟仿真实验室整体解决方案，旨在为高校虚拟仿真实验室建设提供有力支持。
            </p>
        </div>
        <a href="javascript:;">进一步了解></a>
        <div class="b-img">
            <div class="panel-div">
                <img src="../../../assets/images/b-x-2.png">
                <img src="../../../assets/images/b-x-1.png">
            </div>
        </div>
    </div>
</template>

<script type="text/ecmascript-6">
    export default {
        name: 'practiceplatform',
        data() {
            return {
                show:true
            }
        },
        methods: {}
    }
</script>

<style lang="scss" scoped>
    .b-img{
        div{
            img{
                width: 100%;
                height: auto;
                position: absolute;
                top: 0;
                left:0;
            }
            &.panel-div{
                position: relative;
                background-size: 100% 100%;
            }
        }

    }
</style>
