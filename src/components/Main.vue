<template>
  <div>
    <MainServices :numeri="numbers"/>
  </div>
</template>

<script>
import MainServices from './sections/MainServices.vue'

export default {
    name:'Main',
    components:{
        MainServices
    },
    data() {
      return{
        numbers: [
          {
            number: '1.926',
            text: 'FINISHED SESSIONS'
          },
          {
            number: '3.092',
            text: 'ENROLLED LEARNERS'
          },
          {
            number: '200',
            text: 'ONLINE INSTRUCTORS'
          },
          {
            number: '100%',
            text: 'SATISFACTION RATE'
          }
        ],
      }
  }
}
</script>

<style scoped>

    div{
        margin-top: 200px;
    }
</style>