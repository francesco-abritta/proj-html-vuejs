<template>
  <div>
      <div class="title">
          <h2>Let passion and determination be the guide along the way and develop at your own pace that's comfortable</h2>
          <p>FANNIE MORENO</p>
          <p style="color:grey">/Founder & CEO</p>
      </div>
      <div class="numbers">
          <div v-for="(elemento, indice) in numeriServices" :key="indice" class="item">
            <h1>{{elemento.number}}</h1>
            <p>{{elemento.text}}</p>
          </div>
      </div>
      <div class="services">
          <div class="col1">
              <div class="card" v-for="(elemento, indice) in cardServices" :key="'card'+indice" :class="'index'+indice">
                  <div class="text">
                        <h3>{{elemento.titolo}}</h3>
                        <p>{{elemento.par}}</p>
                  </div>
                  <img :src="elemento.image" alt="">
              </div>
          </div>
          
          <div class="col2">
              <div class="block">
                    <p>TOGETHER WE CAN CREATE</p>
                    <h1>Services We <span>Can Provide</span> For My Clients.</h1>
                    <ul>
                        <li v-for="(elem, index) in listServices" :key="'list'+index">
                            <i class="fa-solid fa-check"></i> {{elem.text}}
                        </li>
                    </ul>
                    <button><strong>Get started for free</strong></button>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'MainServices',
    props: {
        numeriServices: Array,
        cardServices: Array,
        listServices: Array
    },
    
}
</script>

<style scoped lang="scss">
  @import '../../assets/vars.scss';
  @import '../../assets/scss/MainServices.scss';
</style>