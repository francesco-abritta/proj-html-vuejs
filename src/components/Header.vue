<template>
  <div>
    <div class="header">
      <div class="logo">

      </div>
      <div class="voices">
        <ul>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>C</li>
          <li>U</li>
        </ul>
      </div>
      <div class="searchbar">
        <input type="text">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {

  }
}
</script>

<style scoped lang="scss">
  @import '../assets/vars.scss';

  .header{
    height: 70px;
    background-color: $header-color;
    color: $header-color-text;
    display: flex;

      .logo{

      }

      .voices{
        background: blue;
          ul{
            list-style: none;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 70px;

              li{
                margin: 0 10px;
              }
          }
      }

      .searchbar{
          display: flex;
          align-items: center;
          background: red;
      }
      


  }

  
</style>
