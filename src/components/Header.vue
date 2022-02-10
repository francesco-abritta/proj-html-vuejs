<template>
  <div>
    <div class="header">
      <HeaderVoices :voices="links"/>      
    </div>
    <Jumbotron />
  </div>
</template>

<script>
import HeaderVoices from './sections/HeaderVoices.vue'
import Jumbotron from './sections/Jumbotron.vue'

export default {
  name: 'Header',
  components: {
    HeaderVoices,
    Jumbotron
  },
  data() {
      return{
        links: [
          {
            text: 'Home'
          },
          {
            text: 'Pages'
          },
          {
            text: 'Courses'
          },
          {
            text: 'Features'
          },
          {
            text: 'Blog'
          },
          {
            text: 'Shop'
          }
        ]
      }
  }
}
</script>

<style scoped lang="scss">
  @import '../assets/vars.scss';
  @import '../assets//scss/Header.scss';
</style>
