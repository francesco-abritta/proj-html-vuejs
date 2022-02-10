<template>
  <div class="cont">
      <div class="titles">
          <p>WANNA TRANSFORM YOUR LIFE?</p>
          <h1>Glad to <span>Help You</span> Learn</h1>
      </div>

      <div class="cards">
          <div class="card" v-for="(elemento, indice) in CardLearn" :key="indice">
              <div class="icon"><img :src="elemento.icon" alt=""></div>
              <div class="title"><h3>{{elemento.title}}</h3></div>
              <div class="par"><p>{{elemento.par}}</p></div>
          </div>
      </div>

      <div class="image">
          <img src="../../assets/img2/home-6-services-image-1024x411.png" alt="">
      </div>

  </div>
</template>

<script>
export default {
    name:'MainLearn',
    props:{
        CardLearn: Array
    }
}
</script>

<style scoped lang="scss">
    @import '../../assets/vars.scss';

    .cont{
        padding: 70px 0;

        .titles{
            text-align: center;

            p{
                font-size: 12px;
                color: grey;
            }

            h1{
                margin: 20px 0px 60px 0px;

                span{
                    color: $lightgreen;
                }
            }
        }

        .cards{
            display: flex;
            justify-content: space-between;

            .card{
                max-width: 23%;

                .title{
                    max-width: 100%;
                }

                h3{
                    margin: 20px 0;
                }

                p{
                    font-size: 13px;
                    margin-top: 15px;
                    color: grey;
                    line-height: 22px;
                }

                img{
                    height: 50px;
                    width: 50px;
                }
            }

            
        }

        .image{
            height: 285px;
            margin-top: 200px;
            display: flex;
            justify-content: center;
            
            img{
                width: 950px;
                height: 381px;
            }
        }
    }
</style>