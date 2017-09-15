<template>
    <div id="banner">
        <data-platform></data-platform>
        <practice-platform></practice-platform>
        <research-platform></research-platform>
        <teach-platform></teach-platform>
        <x-platform></x-platform>
    </div>
</template>

<script type="text/ecmascript-6">

    import DataPlatform from './Product/DataPlatform'
    import PracticePlatform from './Product/PracticePlatform'
    import ResearchPlatform from './Product/ResearchPlatform'
    import XPlatform from './Product/XPlatform'
    import TeachPlatform from './Product/TeachPlatform'

    export default {
        name: 'banner',
        data() {
            return {}
        },
        methods: {

        },
        components:{
            DataPlatform,
            PracticePlatform,
            ResearchPlatform,
            XPlatform,
            TeachPlatform
        }
    }
</script>

<style lang="scss">
    @import "../../style/mixin";

    #banner{
        width: 100%;
        height: 100%;
        box-sizing: border-box;
        padding-top: $head-height;
        position: absolute;
        left: 0;
        top: 0;
        z-index: -1;
        text-align: center;
        overflow: hidden;
        >div{
            position: absolute;
            width: 100%;
            height: 100%;
            left: 0;
            top: $head-height;
        }
        a{
            color: #1AA7B8;
            font-size: 14px;
            margin-top: 10px;
            display: inline-block;
        }
        .b-title{
            font-size: 28px;
            font-weight: bold;
            margin-top: 35px;
            span{
                font-size: 34px;
            }
        }
        .b-title-zh{
            font-size: 22px;
            span{
                font-weight: bold;
            }
        }
        .b-info{
            margin-top: 15px;
            font-size: 14px;
            padding: 0 30px;
        }
        .b-img{
            position: relative;
        }
    }

</style>
