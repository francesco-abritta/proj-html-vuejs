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
    @import '../../assets/scss/MainCourses.scss';
  

</style>