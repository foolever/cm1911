<template>
    <div class="head">
        <div class="nav-box" v-on:touchstart="rotate($event)">
            <span></span>
            <span></span>
        </div>
        <img src="../../assets/logo.png">
        <navigation id="nav"></navigation>
    </div>
</template>

<script type="text/ecmascript-6">
    import Navigation from './Navigation'
    export default {
        name:'head',
        data(){
            return {

            }
        },
        methods:{
            rotate(e){
                let $this=$(e.currentTarget);
                $this.toggleClass("rotate");
                $this.children("span").toggleClass("rotate");
                $("#nav").toggleClass("active")
            }
        },
        components:{
            Navigation
        }
    }
</script>

<style lang="scss">
    @import "../../style/mixin";

    .head{
        width: 100%;
        height: $head-height;
        background: #1AA7B8;
        text-align: center;
        .nav-box{
            width: $head-height;
            height: $head-height;
            float: left;
            transition: all 0.5s;
            transform-origin: 50% 50%;
            background: $bg;
            &.rotate{
                transform: rotate(90deg);
            }
            span{
                margin: 0 auto;
                display: block;
                width: 40%;
                height: 2px;
                background: #fff;
                transform-origin: 50% 50%;
                transition: all 0.5s;
                transition-delay: 0.1s;
                &:first-child{
                    margin-top: 18px;
                    margin-bottom: 5px;
                }
                &.rotate{
                    transform: rotate(-45deg);
                }
                &:first-child.rotate{
                    transform: rotate(45deg);
                    margin-bottom: -2px;
                }
            }
        }
        img{
            height: 100%;
            width: auto;
            margin-left: -$head-height;
        }
        #nav.active{
            height: 100%;
            li{
                opacity: 1;
                transform: translateX(0) translateY(0) scale(1);
            }
        }
    }
</style>
