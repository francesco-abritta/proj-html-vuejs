<template>
  <div id="app">
    <div id="header">
      <Header />
    </div>
    <Main />
    <div class="footer-cont">
      <Footer :address="addressFooter" :explore="exploreFooter" :information="informationFooter"/>
      <div class="buttonTop">
          <a href="#header"><button><i class="fa-solid fa-arrow-up"></i></button></a>
      </div>
    </div>
    
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
  data() {
      return{
        addressFooter: [
          {
            link: '382 NE 191st St # 87394 Miami, FL 33179-3899',
          },
          {
            link: '+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)',
          },
          {
            link: 'support@maxcoach.com',
          },
        ],
        exploreFooter: [
          {
            link: 'Start here',
          },
          {
            link: 'Blog',
          },
          {
            link: 'About us',
          },
          {
            link: 'Success story',
          },
          {
            link: 'Courses',
          },
          {
            link: 'Contact us',
          },
        ],
        informationFooter: [
          {
            link: 'Membership',
          },
          {
            link: 'Purchase guide',
          },
          {
            link: 'Privacy policy',
          },
          {
            link: 'Terms of services',
          },
        ],
    }
  }
}
</script>

<style lang="scss">
  @import './assets/global.scss';
    @import './assets/vars.scss';

  .footer-cont{
    background: $second-background;
    position: relative;
  }

  .buttonTop{
      text-align: end;
      position: absolute;
      bottom: 40px;
      right: 40px;

      button{
        height: 60px;
        width: 60px;
        border-radius: 40px;
        border: 0;
        background: $lightgreen;
        color: white;
        cursor: pointer;

        &:hover{
          background: $header-color;
        }
      }
  }
</style>
