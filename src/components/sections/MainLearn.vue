<template>
  <div class="cont">
      <div class="titles">
          <p>WANNA TRANSFORM YOUR LIFE?</p>
          <h1>Glad to <span>Help You</span> Learn</h1>
      </div>

      <div class="cards">
          <div class="card" v-for="(elemento, indice) in CardLearn" :key="indice">
              <div class="icon"><img :src="elemento.icon" alt=""></div>
              <div class="title"><h3>{{elemento.title}}</h3></div>
              <div class="par"><p>{{elemento.par}}</p></div>
          </div>
      </div>

      <div class="image">
          <img src="../../assets/img2/home-6-services-image-1024x411.png" alt="">
      </div>

  </div>
</template>

<script>
export default {
    name:'MainLearn',
    props:{
        CardLearn: Array
    }
}
</script>

<style scoped lang="scss">
    @import '../../assets/vars.scss';
    @import '../../assets/scss/MainLearn.scss';
</style>