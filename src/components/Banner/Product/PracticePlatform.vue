<template>
    <div class="banner-component data-platform" v-show="show">
        <p class="b-title"><span>T</span>raining platform</p>
        <p class="b-title-zh">实训平台<span>1+N</span></p>
        <div class="b-info">
            <p>
                实训平台运用模块化集中管理理念，通过实训管理平台搭载多种实训系统的模式，旨在建立多学科、多途径、理论实践相结合的全新实训体系，对高校的个性化实训项目进行统一管理，为教学实训的体系化、个性化提供有力支撑。
            </p>
        </div>
        <a href="javascript:;">进一步了解></a>
        <div class="b-img">
            <div class="panel-div">
                <img src="../../../assets/images/b-practice-3.png">
                <img src="../../../assets/images/b-practice-2.png">
                <img src="../../../assets/images/b-practice-1.png">
            </div>
        </div>
    </div>
</template>

<script type="text/ecmascript-6">
    export default {
        name: 'practiceplatform',
        data() {
            return {
                show:false
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
