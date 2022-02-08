<template>
  <div class="voices">
        <ul>
          <li><img src="../../assets/img2/light-logo.png" alt=""></li>

          <li class="links" v-for="(elemento, indice) in voices" :key="indice">{{elemento.text}}<i class="fas fa-chevron-down"></i></li>

          <li class="links" style="margin-left:0;"><i class="fas fa-shopping-cart"></i></li>
          <li class="links"><i class="far fa-user"></i></li>

          <li>
            <span class="input">
              <input type="text" placeholder="Search...">
              <i style="color: #24AE98" class="fas fa-search"></i>
            </span>
          </li>
        </ul>
      </div>
</template>

<script>
export default {
    name:'HeaderVoices',
    props: {
        voices: Array
    }
}
</script>

<style scoped lang="scss">
  img{
    height: 20px;
    margin-right: 140px;
  }

  .voices{
    width: 87%;
      ul{
        list-style: none;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 70px;

        li{
          margin: 0px 2px 0px 15px;
          cursor: pointer;
        }

        .links{
          opacity: 0.5;
        }

        .links:hover{
          opacity: 1;
        }

        .fa-chevron-down{
          font-size:6px; 
          margin-left:3px; 
          vertical-align:middle;
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
</style>