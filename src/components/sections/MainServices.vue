<template>
  <div>
      <div class="title">
          <h2>Let passion and determination be the guide along the way and develop at your own pace that's comfortable</h2>
          <p>FANNIE MORENO</p>
          <p style="color:grey">/Founder & CEO</p>
      </div>
      <div class="numbers">
          <div v-for="(elemento, indice) in numeri" :key="indice" class="item">
            <h1>{{elemento.number}}</h1>
            <p>{{elemento.text}}</p>
          </div>
      </div>
      <div class="services">

      </div>
  </div>
</template>

<script>
export default {
    name: 'MainServices',
    props: {
        numeri: Array
    }
}
</script>

<style scoped lang="scss">
  @import '../../assets/vars.scss';

    .title{
        text-align: center;
        margin: 0 auto;
        max-width: 55%;

        h2{
            line-height: 35px;
        }

        p{
            font-size:10px;
            margin: 25px 0;
        }
    }

    .numbers{
        margin: 100px 0;
        display: flex;
        justify-content: space-between;
        text-align: center;

        h1{
            color: $lightgreen;
        }

        p{
            font-size: 10px;
            color: grey;
            margin-top: 10px;
        }
    }

    
</style>