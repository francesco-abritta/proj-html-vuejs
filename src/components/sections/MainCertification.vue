<template>
  <div>
      <div class="text">
          <p><strong>Start Today for getting <span>Online Certification</span></strong></p>
          <h1>You can be your own guiding star with our help!</h1>
          <button><strong>Get started for free</strong></button>
      </div>
  </div>
</template>

<script>
export default {
    name:'MainCertification'
}
</script>

<style scoped lang="scss">
    @import '../../assets/vars.scss';

    .text{
        text-align: center;

        span{
            color: $lightgreen;
        }

        p{
            margin-bottom: 10px;
        }

        button{
            cursor: pointer;
            padding: 20px 50px;
            border: 0;
            border-radius: 5px;
            background: $lightgreen;
            color: white;
            margin: 45px 0;
        }

        button:hover{
            background: $header-color;
            color: white;
        }
    }
</style>