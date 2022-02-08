<template>
  <div>
    <div class="header">
      
      <div class="voices">
        <ul>
          <li><img src="../assets/img2/light-logo.png" alt=""></li>

          <li>Ciao</li>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>Ciao</li>
          <li>C</li>
          <li>U</li>

          <li>
            <span class="input">
              <input type="text" placeholder="Search...">
              L
            </span>
          </li>
        </ul>
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
    font-size: $header-font-size;

      img{
        height: 20px;
        margin-right: 140px;
      }

      .voices{
        width: 90%;
          ul{
            list-style: none;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 70px;

              li{
                margin: 0 10px;
              }

              .input{
                color: black;
                background: white;
                padding: 10px 10px;
                border-radius: 5px;
                  input{
                    border: 0;
                    width: 100px;
                  }
                  input:focus {
                    outline-width: 0;
                  }
              }

          }
      }
  }

  
</style>
