<template>
    <ul>
        <li v-for="value in list">
            <a v-bind:href="value.router" v-html="value.text">

            </a>
        </li>
    </ul>
</template>

<script type="text/ecmascript-6">
    export default {
        name:'navigation',
        data(){
            return {
                list:[
                    {
                        text:"教学平台1+N",
                        router:'javascript:;'
                    },
                    {
                        text:"实训平台1+N",
                        router:'javascript:;'
                    },
                    {
                        text:"案例平台1+N",
                        router:'javascript:;'
                    },
                    {
                        text:"调查平台1+N",
                        router:'javascript:;'
                    },
                    {
                        text:"数据平台1+N",
                        router:'javascript:;'
                    }
                ],
            }
        },
        methods:{

        }
    }
</script>

<style lang="scss" scoped>
    @import "../../style/mixin";
    ul{
        width: 100%;
        list-style: none;
        box-sizing: border-box;
        text-align: left;
        padding: 0 48px ;
        height: 0;
        overflow: hidden;
        background: rgba(0,0,0,.9);
        position: absolute;
        z-index: 8;
        top: 48px;
        left: 0;
        li{
            border-bottom: 1px solid #333;
            opacity: 0;
            transition: all 0.5s;
            transform: translateX(-5px) translateY(-20px) scale(1.05);
            &:first-child{
                margin-top: 24px;
            }
            &.active{
                a{
                    opacity: 0.65;
                }
            }
            a{
                color: #fff;
                display: block;
                height: 43px;
                line-height: 43px;
            }
            &:nth-of-type(1){
                transition-delay: 0.075s;
            }
            &:nth-of-type(2){
                transition-delay: 0.15s;
            }
            &:nth-of-type(3){
                transition-delay: 0.225s;
            }
            &:nth-of-type(4){
                transition-delay: 0.3s;
            }
            &:nth-of-type(5){
                transition-delay: 0.375s;
            }
        }
    }
</style>
