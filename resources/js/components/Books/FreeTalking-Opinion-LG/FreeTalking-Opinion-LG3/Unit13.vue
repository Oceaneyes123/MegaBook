<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/children-classroom-raising-hands_23-2147659015.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Does Class Size Matter?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class = "line-top-lg">
  </div>
  <h3  class = "lower-header-lg white--text">Topic</h3>

  <div style = "padding : 16px; line-height: 1.6;">

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>Henry :</b></td>
      <td class = "lowertable" >Students in smaller classes tend to have higher test scores. According to a study conducted in Tennessee in 1985, students in classes with up to 17 people had a nearly 8 percent higher reading score compared to those in larger classes. In addition, the study showed that students in smaller classes were more likely to take college entrance exams. This is because of several factors, including less distraction and more time for one-on-one guidance. Plus, according to many surveys, teachers prefer smaller classes, too.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Class size doesn't matter. According to Andreas Schleicher, coordinator of the OECD Program for International Student Assessment, high-performing education systems focus on better teachers, not smaller class sizes. Class sizes in Asia, where academic achievement is generally high, tend to be large. Instead of putting the blame on large class sizes, schools should focus on hiring teachers who can come up with strong teaching plans, manage classrooms, and motivate students. Mediocre teachers want smaller classes because they can’t handle larger ones.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>tend</b> 경향이 있다
        </p>
        <p>
          <b>distraction</b> 집중을 방해하는 것
        </p>
        <p>
          <b>blame</b> 탓
        </p>
        <p>
          <b>mediocre</b> 보통 밖에 안 되는
        </p>
        <p>
          <b>handle</b> 감당하다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >소규모 학급 학생들은 더 높은 시험 점수를 받는 경향이 있습니다. 1985년 테네시 주에서 실시된 한 연구에 따르면, 17명까지 있는 수업의 학생들은 더 큰 수업의 학생들에 비해 거의 8% 높은 읽기 점수를 받았다고 합니다. 게다가, 이 연구는 더 작은 반의 학생들이 대학 입학 시험에 응시할 가능성이 더 높다는 것을 보여주었습니다. 이것은 산만하지 않고 일대일 지도에 더 많은 시간을 할애하는 것을 포함한 몇 가지 요인 때문입니다. 또한, 많은 조사에 따르면, 교사들도 소규모 수업을 선호한다고 합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >학급의 인원수는 중요하지 않습니다 OECD 국제 학생 평가 프로그램의 진행자인 안드레아스 슐리셔에 따르면, 고성능 교육 시스템은 더 작은 학급 크기가 아니라 더 나은 교사들에게 초점을 맞추고 있다고 합니다. 일반적으로 학업 성취도가 높은 아시아 지역의 학급 크기는 큰 경향이 있습니다. 학교들은 큰 학급 규모에 책임을 물을 것이 아니라, 강력한 교육 계획을 세우고, 교실을 관리하고, 학생들에게 동기를 부여할 수 있는 교사들을 고용하는 데 초점을 맞춰야 합니다. 보통의 교사들은 더 큰 수업을 감당할 수 없기 때문에 소규모의 수업을 원합니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Does class size matter? Why or why not?</li>
          <li>As a student, in what class size do you belong? A big or a smaller class size? How did it affect your learning experience?</li>
          <li>Does a smaller class size guarantee higher achievement among students? Why or why not?</li>
        </ol>

      </div>

    </div>


  </v-layout>
</v-container>
</div>



</template>



<script>
export default {

  props: ['fontSize'],

  data(){

    return{
      showTitle:false


    }

  },

mounted(){
  this.showTitle=true
},

  beforeMount(){



  },

  methods:{


  },

  watch:{

    fontSize(current, old){

      console.log(current, 'current')
      console.log(old, 'previous')


    }
  }
}
</script>

<style scoped lang="css">

</style>
