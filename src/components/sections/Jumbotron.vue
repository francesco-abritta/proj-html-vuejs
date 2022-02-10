<template>
  <div>
      <div class="jumbo">
          <h1>Learn At Your Own Pace!</h1>
          <p>Get teamed up with people of the same will.</p>
          <button><strong>Get started for free</strong></button>
          <div class="images">
            <div class="left"><img src="../../assets/img1/home-6-hero-left-person.png" alt=""></div>
            <div class="center"><img src="../../assets/img1/video-screen.png" alt=""></div>
            <div class="right"><img src="../../assets/img1/home-6-hero-right-person.png" alt=""></div>
          </div>
          <div class="sideMenu">
              <div><i class="fa-solid fa-ruler-combined"></i></div>
              <div><i class="fa-solid fa-circle-radiation"></i></div>
              <div><i class="fa-solid fa-book"></i></div>
              <div><i class="fa-solid fa-cart-shopping"></i></div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:'Jumbotron'
}
</script>

<style scoped lang="scss">
  @import '../../assets/vars.scss';
  .jumbo{
      background: $header-color;
      color: $header-color-text;
      height: 550px;
      text-align: center;
      padding-top: 30px;
      position: relative;

      .sideMenu{
          color: black;
          position: absolute;
          right: 0;
          top: 10%;
          padding: 0px 10px;
          background: white;
          border-radius: 5px 0px 0px 5px;

          div{
              margin: 15px 0;
          }
      }
      p{
          font-size: 14px;
          color: grey;
          margin: 20px 0;
      }
      button{
          padding: 20px 30px;
          border: 0;
          border-radius: 5px;
          background: $lightgreen;
          color: white;
          cursor: pointer;
      }
      button:hover{
          background: white;
          color: $lightgreen;
      }
      img{
          height: 400px;
      }
      .images{
          padding-top: 30px;
      }
      .center, .left, .right{
          display: inline-block;
          height: 400px;
      }
      .center{
          height: 460px;
          padding: 30px;
          background: white;
          border-radius: 20px;
        //   border: 1px solid grey;
          box-shadow: 0px 10px 10px #dedede;
      }
      .left, .right{
          position: relative;
      }
      .right img{
          position: absolute;
          top: 200px;
          right: 0;
      }
      .right{
          width: 260px;
          overflow: hidden;
      }
      .left img{
          position: absolute;
          top: 0;
          right: -65px;
      }
      .left{
          width: 260px;
          overflow: hidden;
      }
  }
</style>