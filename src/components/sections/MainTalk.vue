<template>
  <div class="cont">
      <div class="title">
          <h1>Why People Talk About <span>MaxCoach</span>?</h1>
      </div>
      <div class="main">
          <div class="image">
              <div class="photo">
                  
              </div>
              <img src="../../assets/img2/maxcoach-shape-05-100x100.png" alt="">
          </div>
          <div class="phrase">
              <div class="text">
                  <p>I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.</p>
              </div>
              <div class="credits">
                  <p class="person">MINA HOLLACE</p>
                  <p class="job">/Freelancer</p>
              </div>
          </div>
      </div>
      <div class="sponsor">

      </div>
  </div>
</template>

<script>
export default {
    name:'MainTalk'
}
</script>

<style scoped lang="scss">
  @import '../../assets/vars.scss';

    .cont{
        margin: 50px 0;

        .title{
            text-align: center;

            span{
                color: $lightgreen;
            }
        }

        .main{
            display: flex;
            justify-content: center;
            margin: 50px 0;
        }

        .image{
            background: red;
            position: relative;
            height: 220px;
            margin-right: 60px;

            img{
                position: absolute;
                top: 110px;
                right: 0;
            }

            .photo{
                border-radius: 100px;
                width: 170px;
                height: 170px;
                overflow: hidden;
                background: blue;
            }

        }

        .phrase{
            max-width: 70%;

            .text p{
                font-size: 30px;
                line-height: 40px;
                margin-bottom: 35px;
            }

            .person{
                font-weight: bold;
                font-size: 13px;
                margin-bottom: 15px;
            }

            .job{
                font-size: 12px;
                color: grey;
            }
        }

        
    }
</style>