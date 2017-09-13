<template>
  <div id="app">
      <head-top></head-top>
  </div>
</template>

<script>
import './plugins/jquery.min'
import headTop from './components/Header/Head'

export default {
    name: 'app',
    components:{
        headTop
    }
}
</script>

<style lang="scss">
    *{
        margin: 0;
        padding: 0;
        text-decoration: none;
    }
    .rotate{
        well-change:'transform'
    }
    #app {

    }
</style>
