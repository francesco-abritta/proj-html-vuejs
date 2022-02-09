<template>
  <div>
      <div class="section">
        <div class="titles">
            <p>CHOOSE A COURSE TO GET STARTED</p>
            <h1>Latest Featured <span>Courses</span></h1>
        </div>

        <div class="cards">
            <div class="card" v-for="(elemento, indice) in infoCourses" :key="indice">
                <div class="image" :class="'indice'+indice">
                    <!-- <img src="../../assets/img2/course-02-480x298.jpg" alt=""> -->
                    <!-- <img src="../../assets/img2/stock-full-hd-03-480x298.jpg" alt=""> -->
                </div>
                
                <div class="text">
                    <div class="price">
                        <h2>{{elemento.price}}</h2>
                    </div>
                    <div class="description">
                        <p>{{elemento.work}}</p>
                    </div>
                    <div class="info">
                        <div class="icon1">
                            <i class="fa-solid fa-file-lines"></i> {{elemento.data1}} Lessons
                        </div>
                        <div class="icon2">
                            <i class="fa-solid fa-user"></i> {{elemento.data2}} Students
                        </div>
                    </div>
                </div>
            </div>
            
        </div>

        <div class="button">
            <button><strong>View all courses <i class="fa-solid fa-arrow-right"></i></strong></button>
        </div>
      </div>
      
  </div>
</template>

<script>


export default {
    name:'MainCourses',
    props:{
        infoCourses: Array,
    }
}
</script>

<style scoped lang="scss">

  @import '../../assets/vars.scss';

    .section{
        padding: 50px 0;

        .titles{
            text-align: center;

            p{
                font-size: 12px;
            }

            h1{
                margin: 20px 0;

                span{
                    color: $lightgreen;
                }
            }
        }

        .cards{
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 50px;


            .card{
            display: flex;
            align-items: center;
            max-width: 47%;
            padding: 5px;
            line-height: 25px;
            margin-bottom: 20px;
            margin-right: 20px;
            border-radius: 15px;
            

            
            .image{
                border-radius: 100px;
                width: 140px;
                height: 140px;
                overflow: hidden;
                position: relative;

                // img{
                //     position: absolute;
                //     top: 50%;
                //     left: 50%;
                //     transform: translate(-50%, -50%);
                // }
            }

        
            .text{
                margin-left: 20px;

                .price{
                    color: $lightgreen;
                }

                .description{
                    margin: 10px 0;
                    font-weight: bold;
                    width: 270px;
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
            .card:hover{
                background: white;
                cursor: pointer;
            }

            
    }


    .button{
        text-align: center;
        margin-top: 20px;
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
        
}
.indice0{
    background-image: url('../../assets/img2/course-02-480x298.jpg');
    background-position: center;
    background-size: cover;
}
.indice1{
    background-image: url('../../assets/img2/stock-full-hd-03-480x298.jpg');
    background-position: center;
    background-size: cover;
}
.indice2{
    background-image: url('../../assets/img2/stock-full-hd-04-480x298.jpg');
    background-position: center;
    background-size: cover;
}
.indice3{
    background-image: url('../../assets/img2/stock-full-hd-06-480x298.jpg');
    background-position: center;
    background-size: cover;
}
.indice4{
    background-image: url('../../assets/img2/course-featured-image-01-480x298.jpg');
    background-position: center;
    background-size: cover;
}
.indice5{
    background-image: url('../../assets/img2/stock-full-hd-05-480x298.jpg');
    background-position: center;
    background-size: cover;
}

</style>