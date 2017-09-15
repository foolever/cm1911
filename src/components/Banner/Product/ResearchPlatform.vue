<template>
    <div class="banner-component data-platform" v-show="show">
        <p class="b-title"><span>I</span>nvestigation platform</p>
        <p class="b-title-zh">调查平台<span>1+N</span></p>
        <div class="b-info">
            <p>
                调查平台1+N融合传统调查方式与互联网技术及通信技术，是大数据时代获取数据、分析数据不可或缺的工具。调查平台以1个基础模块与N款扩展模块的方式组合，可以实现电访、面访等多种途径的调查。并且，通过本地服务器部署，可防止利用第三方平台造成数据泄露，保障数据信息的安全。
            </p>
        </div>
        <a href="javascript:;">进一步了解></a>
        <div class="b-img">
            <div class="panel-div">
                <img src="../../../assets/images/b-research-2.png"/>
                <div class="wave-div">
                    <img src="../../../assets/images/b-research-1.png">
                </div>
            </div>
        </div>
    </div>
</template>

<script type="text/ecmascript-6">
    export default {
        name: 'researchplatform',
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
            }
            &.wave-div{
                width: 100%;
                height: 100%;
                overflow: hidden;
                position: absolute;
                top: 0;
                left: 0;
                background: url("../../../assets/images/b-research-1.png") top left no-repeat;
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
