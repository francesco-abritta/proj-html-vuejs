<template>
  <div id="app">
    <Header />
    <Main />
    <div class="footer-cont">
      <Footer :address="addressFooter" :explore="exploreFooter" :information="informationFooter"/>
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
  }
</style>
