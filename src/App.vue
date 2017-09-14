<template>
  <div id="app">
      <head-top></head-top>
      <banner></banner>
  </div>
</template>

<script>
import './plugins/jquery.min'
import headTop from './components/Header/Head'
import banner from './components/Banner/Banner'

export default {
    name: 'app',
    components:{
        headTop,
        banner
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
