<template>
  <div class="contenitore">
      <div class="footer">
          <div class="left">
                <ul class="address">
                    <li><strong>Address</strong></li>
                    <li><p>ciaociaociaociaociaocio</p></li>
                    <li><p>ciaociaociaociaociaocio</p></li>
                    <li><p>ciaociaociaociaociaocio</p></li>
                </ul>
                <ul class="icon">
                    <li><i class="fa-brands fa-facebook-square"></i></li>
                    <li><i class="fa-brands fa-twitter"></i></li>
                    <li><i class="fa-brands fa-instagram"></i></li>
                    <li><i class="fa-brands fa-linkedin"></i></li>
                </ul>
          </div>

          <div class="right">
                <div>
                    <h3>Explore</h3>
                    <div class="explore">
                        <ul class="explore-left">
                            <li><p>ciaociao</p></li>
                            <li><p>ciaociao</p></li>
                            <li><p>ciaociao</p></li>
                        </ul>

                        <ul class="explore-right">
                            <li><p>ciaociao</p></li>
                            <li><p>ciaociao</p></li>
                            <li><p>ciaociao</p></li>
                        </ul>

                    </div>
                </div>
                <div>
                    <h3>Information</h3>
                    <ul class="information">
                        <li><p>ciaociaociaociaociaocio</p></li>
                        <li><p>ciaociaociaociaociaocio</p></li>
                        <li><p>ciaociaociaociaociaocio</p></li>
                        <li><p>ciaociaociaociaociaocio</p></li>
                    </ul>
                </div>
                
          </div>
          
      </div>
  </div>
</template>

<script>
export default {
    name:'Footer'
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
                    margin: 14px 0;
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
                    min-width: 200%;
                    max-height: 120px;
                    display: flex;
                    flex-direction: column;
                    flex-wrap: wrap;
                    align-content: space-between;
                    
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
    }
</style>