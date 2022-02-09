<template>
  <div>
    <MainServices :numeri="numbers" :cardServices="servicesCard" :listServices="servicesList"/>
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

        servicesCard: [
          {
            titolo: 'Graphic Design',
            par: 'Have a passion for graphics and arts? Show your talents whit confidence and self assertiveness.',
            image: require('../assets/img2/home-6-service-image-01.png')
          },
          {
            titolo: 'Business Administration',
            par: 'Learners are encouraged to study the mechanism and structure of system administration.',
            image: require('../assets/img2/home-6-service-image-02.png')
          },
          {
            titolo: 'Idea Discussion',
            par: 'Get teamed up with the specialists who work and teach coding for years at famous universities',
            image: require('../assets/img2/home-6-service-image-03.png')
          },
          {
            titolo: 'Web Development',
            par: 'Learn to start building a webpage from scratch. You decide your own pace, course and speed',
            image: require('../assets/img2/home-6-service-image-04.png')
          }
        ],
        
        servicesList: [
          {
            text: 'Select & costumize courses to your prefernces'
          },
          {
            text: 'Change the tutor and male arrangements'
          },
          {
            text: 'Partecipate in events to join others'
          },
          {
            text: 'Get the desired certificate delivered at house'
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