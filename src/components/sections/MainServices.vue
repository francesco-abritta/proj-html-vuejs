<template>
  <div>
      <div class="title">
          <h2>Let passion and determination be the guide along the way and develop at your own pace that's comfortable</h2>
          <p>FANNIE MORENO</p>
          <p style="color:grey">/Founder & CEO</p>
      </div>
      <div class="numbers">
          <div v-for="(elemento, indice) in numeri" :key="indice" class="item">
            <h1>{{elemento.number}}</h1>
            <p>{{elemento.text}}</p>
          </div>
      </div>
      <div class="services">
          <div class="col1">
              <div class="card">
                  <h3>Graphic Design</h3>
                  <p>Have a passion for graphics and arts? Show your talents whit confidence and self assertiveness.</p>
                  <img src="../../assets/img2/home-6-service-image-01.png" alt="">
              </div>
              <div class="card">
                  <h3>Graphic Design</h3>
                  <p>Have a passion for graphics and arts? Show your talents whit confidence and self assertiveness.</p>
                  <img src="../../assets/img2/home-6-service-image-01.png" alt="">
              </div>
              <div class="card">
                  <h3>Graphic Design</h3>
                  <p>Have a passion for graphics and arts? Show your talents whit confidence and self assertiveness.</p>
                  <img src="../../assets/img2/home-6-service-image-01.png" alt="">
              </div>
              <div class="card">
                  <h3>Graphic Design</h3>
                  <p>Have a passion for graphics and arts? Show your talents whit confidence and self assertiveness.</p>
                  <img src="../../assets/img2/home-6-service-image-01.png" alt="">
              </div>
          </div>
          
          <div class="col2">
              <div class="block">
                    <p>TOGETHER WE CAN CREATE</p>
                    <h1>Services We <span>Can Provide</span> For My Clients.</h1>
                    <ul>
                        <li>
                            <i class="fa-solid fa-check"></i> Select & costumize courses to your preferences
                        </li>
                        <li>
                            <i class="fa-solid fa-check"></i> Select & costumize courses to your preferences
                        </li>
                        <li>
                            <i class="fa-solid fa-check"></i> Select & costumize courses to your preferences
                        </li>
                        <li>
                            <i class="fa-solid fa-check"></i> Select & costumize courses to your preferences
                        </li>
                    </ul>
                    <button><strong>Get started for free</strong></button>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'MainServices',
    props: {
        numeri: Array,
        // cardServices: Array,
        // listServices: Array
    }
}
</script>

<style scoped lang="scss">
  @import '../../assets/vars.scss';

    .title{
        text-align: center;
        margin: 0px auto;
        max-width: 55%;

        h2{
            line-height: 35px;
            margin-top: 300px;
        }

        p{
            font-size:10px;
            margin: 25px 0;
        }
    }

    .numbers{
        margin: 100px 0;
        display: flex;
        justify-content: space-between;
        text-align: center;

        h1{
            color: $lightgreen;
        }

        p{
            font-size: 10px;
            color: grey;
            margin-top: 10px;
        }
    }

    .services{
        margin-bottom: 50px;
        display: flex;
        justify-content: space-between;

        .col1{
            width: 440px;
            display: flex;
            flex-wrap: wrap;

            .card{
                width: 200px;
                height: 315px;
                box-shadow: 0px 0px 25px 0px #8d8c8c;
                border-radius: 10px;
                margin: 10px;
                // margin-top: 45px;

                h3{
                    padding: 20px 10px;
                }

                p{
                    padding: 0 10px;
                    color: grey;
                    font-size: 14px;
                    line-height: 22px;
                }

                img{
                    width: 200px;
                }

            }
        }

        .col2{
            width: 400px;
            display: flex;
            align-items: center;

            .block *{
                margin: 20px 0;
            }

            p{
                font-size: 14px;
                color: grey;
            }

            h1{
                font-size: 40px;

                span{
                    color: $lightgreen;
                }
            }

            ul{
                list-style: none;
                color: grey;
            }

            .fa-check{
                margin: 0px 10px 0px 0px;
                color: $lightgreen;
            }
        }
    }

    

    button{
        padding: 20px 30px;
        border: 0;
        border-radius: 5px;
        background: $lightgreen;
        color: white;
    }

    
</style>