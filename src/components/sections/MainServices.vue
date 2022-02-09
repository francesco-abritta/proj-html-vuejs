<template>
  <div>
      <div class="title">
          <h2>Let passion and determination be the guide along the way and develop at your own pace that's comfortable</h2>
          <p>FANNIE MORENO</p>
          <p style="color:grey">/Founder & CEO</p>
      </div>
      <div class="numbers">
          <div v-for="(elemento, indice) in numeriServices" :key="indice" class="item">
            <h1>{{elemento.number}}</h1>
            <p>{{elemento.text}}</p>
          </div>
      </div>
      <div class="services">
          <div class="col1">
              <div class="card" v-for="(elemento, indice) in cardServices" :key="'card'+indice" :class="'index'+indice">
                  <div class="text">
                        <h3>{{elemento.titolo}}</h3>
                        <p>{{elemento.par}}</p>
                  </div>
                  <img :src="elemento.image" alt="">
              </div>
          </div>
          
          <div class="col2">
              <div class="block">
                    <p>TOGETHER WE CAN CREATE</p>
                    <h1>Services We <span>Can Provide</span> For My Clients.</h1>
                    <ul>
                        <li v-for="(elem, index) in listServices" :key="'list'+index">
                            <i class="fa-solid fa-check"></i> {{elem.text}}
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
        numeriServices: Array,
        cardServices: Array,
        listServices: Array
    },
    
}
</script>

<style scoped lang="scss">
  @import '../../assets/vars.scss';

    .title{
        text-align: center;
        margin: 0px auto;
        max-width: 80%;

        h2{
            line-height: 35px;
            margin-top: 300px;
            font-size: 35px;
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
            font-size: 35px;
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
        justify-content: center;

        .col1{
            width: 500px;
            display: flex;
            flex-wrap: wrap;

            .card{
                display: flex;
                flex-direction: column;
                width: 220px;
                height: 350px;
                box-shadow: 0px 0px 25px 0px #8d8c8c;
                border-radius: 10px;
                margin: 10px;

                h3{
                    padding: 20px 20px;
                    font-size: 15px;
                }

                p{
                    padding: 0 20px;
                    color: grey;
                    font-size: 14px;
                    line-height: 22px;
                }

                img{
                    width: 200px;
                    height: 180px;
                }

            }

            
        }

        

        .col2{
            width: 400px;
            display: flex;
            align-items: center;
            margin-left: 50px;

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
        cursor: pointer;
        padding: 20px 30px;
        border: 0;
        border-radius: 5px;
        background: $lightgreen;
        color: white;
    }

    button:hover{
        background: $header-color;
        color: white;
    }

    .index1, .index3{
        margin-top: 45px !important;
    }

    .index2, .index3{
        display: flex;
        flex-direction: column-reverse !important;
    }

    .index1 img, .index2 img{
        width: 150px !important;
    }

    .index1{
        align-items: center;
    }

    .index3 img{
        height: 160px !important;
        width: 180px !important;
    }

    .index3{
        align-items: center;
    }

    
</style>