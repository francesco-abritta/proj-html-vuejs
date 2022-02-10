<template>
  <div class="contenitore">
      <div class="footer">
          <div class="left">
                <h3>Address</h3>
                <ul class="address">
                    <li v-for="(elemento,indice) in address" :key="indice+'address'"><p>{{elemento.link}}</p></li>
                </ul>
                <ul class="icon">
                    <li><i class="fa-brands fa-facebook-square"></i></li>
                    <li><i class="fa-brands fa-twitter"></i></li>
                    <li><i class="fa-brands fa-instagram"></i></li>
                    <li><i class="fa-brands fa-linkedin"></i></li>
                </ul>
          </div>

          <div class="right">
                    <div class="explore">
                        
                        <h3>Explore</h3>
                        <ul class="exploreList">
                            <li v-for="(elemento,indice) in explore" :key="indice+'explore'"><p>{{elemento.link}}</p></li>
                        </ul>


                    </div>
                <div class="info">
                    <h3>Information</h3>
                    <ul class="information">
                        <li v-for="(elemento,indice) in information" :key="indice+'information'"><p>{{elemento.link}}</p></li>
                    </ul>
                </div>
          </div>
      </div>

      <div class="final">
            <p><i class="fa-solid fa-copyright"></i> 2020 MaxCoach, All Rights Reserved</p>
      </div>
  </div>
</template>

<script>
export default {
    name:'Footer',
    props:{
        address: Array,
        explore: Array,
        information: Array
    }
}
</script>

<style scoped lang="scss">
    .contenitore{
        margin: 0 auto;
        max-width: 65%;
        padding: 80px 0;

        .footer, .right{
            display: flex;
            justify-content: space-between;

            ul{
                list-style: none;

                p{
                    opacity: 0.5;
                    margin-bottom: 28px;
                    font-size: 14px;
                }

                p:hover, li:hover{
                    opacity: 1;
                    cursor: pointer;
                }
            }

            .right{
                width: 50%;

                .explore{
                    max-height: 120px;

                    p{
                        margin: 14px 0 !important;
                    }

                    .exploreList{
                        height: 150px;
                        width: 250px;
                        display: flex;
                        flex-direction: column;
                        flex-wrap: wrap;
                    }
                    
                    li{
                        margin-right: 90px;
                    }
                }
            }

            .icon{
                display: flex;
                margin-top: 30px;

                .fa-facebook-square, .fa-twitter, .fa-instagram, .fa-linkedin{
                    height: 30px;
                    margin-right: 20px;
                    opacity: 0.5;

                    &:hover{
                        opacity: 1;
                    }
                }
            }

        }
        .final{
                text-align: center;
                margin-top: 50px;

                p{
                    font-size: 10px;
                    color: rgb(160, 159, 159);
                }
        }

        .info h3, .left h3{
            margin-bottom: 14px !important;
        }
    }
</style>