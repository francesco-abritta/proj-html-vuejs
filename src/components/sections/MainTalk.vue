<template>
  <div class="cont">
      <div class="title">
          <h1>Why People Talk About <span>MaxCoach</span>?</h1>
      </div>
      <div class="main">
          <div class="image">
              <div class="photo">
                  
              </div>
              <img src="../../assets/img2/maxcoach-shape-05-100x100.png" alt="">
          </div>
          <div class="phrase">
              <div class="text">
                  <p>I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.</p>
              </div>
              <div class="credits">
                  <p class="person">MINA HOLLACE</p>
                  <p class="job">/Freelancer</p>
              </div>
          </div>
      </div>
      <div class="sponsor">
          <img v-for="(elemento, indice) in imagesTalk" :key="'indiceImage'+indice" :src="elemento.image">
      </div>
  </div>
</template>

<script>
export default {
    name:'MainTalk',
    props:{
        imagesTalk: Array
    }
}
</script>

<style scoped lang="scss">
  @import '../../assets/vars.scss';
  @import '../../assets/scss/MainTalk.scss';
</style>