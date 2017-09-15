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
        methods: {},
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
    }

</style>
