<template>
    <div class="banner-component data-platform" v-show="show">
        <p class="b-title"><span>D</span>ata platform</p>
        <p class="b-title-zh">数据平台<span>1+N</span></p>
        <div class="b-info">
            <p>数据平台1+N是基于云计算架构的生产实践创新型数据科学与大数据平台，整体平台以1个数据管理软件为核心，N多的数据库资源为依托，可以帮助高校快速建立数据科学与大数据资源。</p>
        </div>
        <a href="javascript:;">进一步了解></a>
        <div class="b-img">
            <div class="panel-div">
                <img src="../../../assets/images/b-data-2.png"/>
                <div class="wave-div">
                    <img src="../../../assets/images/b-data-1.png">
                </div>
            </div>
        </div>
    </div>
</template>

<script type="text/ecmascript-6">
    export default {
        name: 'dataplatform',
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
            }
            &.panel-div{
                position: relative;
                background: url("../../../assets/images/b-data-3.png") top left no-repeat;
                background-size: 100% 100%;
            }
            &.wave-div{
                width: 100%;
                height: 100%;
                overflow: hidden;
                position: absolute;
                top: 0;
                left: 0;
                background: url("../../../assets/images/b-data-1.png") top left no-repeat;
                background-size: auto 100%;
                img{
                    width: auto;
                    visibility: hidden;
                    height: 100%;
                }
            }
        }

    }
</style>
