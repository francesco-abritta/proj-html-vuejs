<template>
  <div class="total">
      <div class="services">
        <div class="contenitore">
            <MainServices :numeriServices="servicesNumbers" :cardServices="servicesCard" :listServices="servicesList"/>
        </div>
      </div>
      
      <div class="courses">
        <div class="contenitore">
            <MainCourses :infoCourses="coursesInfo"/>
        </div>
      </div>

      <div class="talk">
        <div class="contenitore">
            <MainTalk :imagesTalk="talkImages"/>
        </div>
      </div>

      <div class="blogs">
        <div class="contenitore">
            <MainBlogs :CardBlogs="blogsCard"/>
        </div>
      </div>

      <div class="learn">
        <div class="contenitore">
            <MainLearn :CardLearn="learnCard"/>
        </div>
      </div>

      <div class="certification">
        <div class="contenitore">
            <MainCertification />
        </div>
      </div>
      
  </div>
</template>

<script>
import MainServices from './sections/MainServices.vue'
import MainCourses from './sections/MainCourses.vue'
import MainTalk from './sections/MainTalk.vue'
import MainBlogs from './sections/MainBlogs.vue'
import MainLearn from './sections/MainLearn.vue'
import MainCertification from './sections/MainCertification.vue'

export default {
    name:'Main',
    components:{
        MainServices,
        MainCourses,
        MainTalk,
        MainBlogs,
        MainLearn,
        MainCertification
    },
    data() {
      return{
        servicesNumbers: [
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

        coursesInfo: [
          {
            price: '$40.00',
            work: 'Learning to Write as a Professional Author',
            data1: '17',
            data2: '50'
          },
          {
            price: 'Free',
            work: 'Costumer-centric Info-Tech Strategies',
            data1: '24',
            data2: '769'
          },
          {
            price: '$19.00',
            work: 'Open Programming Courses for Everyone: Phyton',
            data1: '17',
            data2: '62'
          },
          {
            price: '$26.00',
            work: 'Academic Listening and Note-taking',
            data1: '14',
            data2: '67'
          },
          {
            price: '$39.00',
            work: 'Master jQuery in a Short Period of Time',
            data1: '6',
            data2: '51'
          },
          {
            price: '$59.00',
            work: 'Introduction to Javascript for Beginners',
            data1: '14',
            data2: '76'
          },
        ],

        talkImages: [
          {
            image: require('../assets/img2/client-logo-colored-01.png')
          },
          {
            image: require('../assets/img2/client-logo-colored-02.png')
          },
          {
            image: require('../assets/img2/client-logo-colored-03.png')
          },
          {
            image: require('../assets/img2/client-logo-colored-04.png')
          },
          {
            image: require('../assets/img2/client-logo-colored-05.png')
          },
          {
            image: require('../assets/img2/client-logo-colored-06.png')
          },
        ],

        blogsCard: [
          {
            image: require('../assets/img2/artist-blog-03-480x325.jpeg'),
            role: 'ARTIST',
            job: 'Brush Strokes Energize Trees in Paintings',
            date: 'May 15, 2020',
            views: '688',
          },
          {
            image: require('../assets/img2/artist-blog-01-480x325.jpg'),
            role: 'ARTIST',
            job: 'Pocket-Sized Notebooks Hold Miniature Paintings',
            date: 'May 15, 2020',
            views: '603',
          },
          {
            image: require('../assets/img2/artist-blog-02-480x325.jpg'),
            role: 'ARTIST',
            job: 'Connection Between Self-Portraits and Identity',
            date: 'May 15, 2020',
            views: '397',
          },
        ],
        learnCard: [
          {
            icon: require('../assets/img1/flag.png'),
            title: 'Idea Discussion',
            par: 'Get teamed up with the specialists who work and teach coding for years at famous univeristies',
          },
          {
            icon: require('../assets/img1/setting.jpeg'),
            title: 'Web Development',
            par: 'Learn to start building a webpage from scratch. You decide your own pace, course and speed.',
          },
          {
            icon: require('../assets/img1/donut.png'),
            title: 'System Administration',
            par: 'Learners are encouraged to study the mechanism and structure of system administration.',
          },
          {
            icon: require('../assets/img1/desktop.png'),
            title: 'Grapich Design',
            par: 'Have a passion for graphics arts? Show your talents with confidence and self-assertiveness',
          }
        ],
      }
  }
}
</script>

<style scoped>
    .total{
        margin-top: 200px;
    }

    .contenitore{
        margin: 0 auto;
        max-width: 65%;
    }

    .courses, .blogs{
        background: #F5F7FA;
    }

    .learn{
      box-shadow: inset 0px -50px 50px 25px #EFF1F4;
    }

    .certification{
      padding: 80px 0px 50px 0px;
    }
</style>