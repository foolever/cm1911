<template>
    <div id="banner">

    </div>
</template>

<script type="text/ecmascript-6">
    export default {
        name: 'banner',
        data() {
            return {}
        },
        methods: {}
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
