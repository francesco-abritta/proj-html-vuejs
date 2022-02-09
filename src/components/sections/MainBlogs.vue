<template>
  <div class="cont">
      <div class="titles">
          <p>ENJOY READING ON MAXCOACH</p>
          <h1>Latest on <span>Our Blogs</span></h1>
      </div>

      <div class="cards">
          <div class="card" v-for="(elemento, indice) in CardBlogs" :key="indice">
              <img :src="elemento.image" alt="">
              <div class="artist"><p>{{elemento.role}}</p></div>
              <div class="job"><h3>{{elemento.job}}</h3></div>
              <div class="info">
                <div class="icon1">
                    <i class="fa-solid fa-calendar"></i> {{elemento.date}}
                </div>
                <div class="icon2">
                    <i class="fa-solid fa-eye"></i> {{elemento.views}} views
                </div>
            </div>
          </div>
          
      </div>

  </div>
</template>

<script>
export default {
    name:'MainBlogs',
    props:{
        CardBlogs: Array
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
                max-width: 30%;

                img{
                    max-width: 100%;
                    border-radius: 5px;
                }

                p{
                    font-size: 12px;
                    margin-top: 15px;
                    color: grey;
                }

                h3{
                    line-height: 30px;
                    margin: 10px 0;
                }

                .info{
                    display: flex;
                    font-size: 13px;
                    .icon1, .icon2{
                        margin-right: 15px;
                        color: grey;
                    }
                }
            }

            
        }
    }
</style>