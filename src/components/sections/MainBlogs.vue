<template>
  <div class="cont">
      <div class="titles">
          <p>ENJOY READING ON MAXCOACH</p>
          <h1>Latest on <span>Our Blogs</span></h1>
      </div>

      <div class="cards">
          <div class="card" v-for="(elemento, indice) in CardBlogs" :key="indice">
              <img :src="elemento.image" alt="">
              <div class="artist"><p>{{elemento.role}}</p></div>
              <div class="job"><h3>{{elemento.job}}</h3></div>
              <div class="info">
                <div class="icon1">
                    <i class="fa-solid fa-calendar"></i> {{elemento.date}}
                </div>
                <div class="icon2">
                    <i class="fa-solid fa-eye"></i> {{elemento.views}} views
                </div>
            </div>
          </div>
          
      </div>

  </div>
</template>

<script>
export default {
    name:'MainBlogs',
    props:{
        CardBlogs: Array
    }
}
</script>

<style scoped lang="scss">

  @import '../../assets/vars.scss';
  @import '../../assets/scss/MainBlogs.scss';

    
</style>