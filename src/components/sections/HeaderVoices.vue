<template>
  <div class="voices">
        <ul>
          <li><img src="../../assets/img2/light-logo.png" alt=""></li>

          <li class="links" v-for="(elemento, indice) in voices" :key="indice">{{elemento.text}}<i class="fas fa-chevron-down"></i></li>

          <li class="links" style="margin-left:0;"><i class="fas fa-shopping-cart"></i></li>
          <li class="links"><i class="far fa-user"></i></li>

          <li>
            <span class="input">
              <input type="text" placeholder="Search...">
              <i style="color: #24AE98" class="fas fa-search"></i>
            </span>
          </li>
        </ul>
      </div>
</template>

<script>
export default {
    name:'HeaderVoices',
    props: {
        voices: Array
    }
}
</script>

<style scoped lang="scss">

  @import '../../assets/scss/HeaderVoices.scss';

  
</style>