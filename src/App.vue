<template>
  <div id="app">
    <Header />
    <div class="contenitore">
      <Main />
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main
  }
}
</script>

<style lang="scss">
  @import './assets/global.scss';
  .contenitore{
    margin: 0 auto;
    max-width: 65%;
  }
</style>
