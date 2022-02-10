<template>
  <div class="contenitore">
      <div class="footer">
          <div class="left">
                <h3>Address</h3>
                <ul class="address">
                    <li v-for="(elemento,indice) in address" :key="indice+'address'"><p>{{elemento.link}}</p></li>
                </ul>
                <ul class="icon">
                    <li><i class="fa-brands fa-facebook-square"></i></li>
                    <li><i class="fa-brands fa-twitter"></i></li>
                    <li><i class="fa-brands fa-instagram"></i></li>
                    <li><i class="fa-brands fa-linkedin"></i></li>
                </ul>
          </div>

          <div class="right">
                    <div class="explore">
                        
                        <h3>Explore</h3>
                        <ul class="exploreList">
                            <li v-for="(elemento,indice) in explore" :key="indice+'explore'"><p>{{elemento.link}}</p></li>
                        </ul>


                    </div>
                <div class="info">
                    <h3>Information</h3>
                    <ul class="information">
                        <li v-for="(elemento,indice) in information" :key="indice+'information'"><p>{{elemento.link}}</p></li>
                    </ul>
                </div>
          </div>
      </div>

      <div class="final">
            <p><i class="fa-solid fa-copyright"></i> 2020 MaxCoach, All Rights Reserved</p>
      </div>
  </div>
</template>

<script>
export default {
    name:'Footer',
    props:{
        address: Array,
        explore: Array,
        information: Array
    }
}
</script>

<style scoped lang="scss">
  @import '../assets/scss/Footer.scss';
</style>