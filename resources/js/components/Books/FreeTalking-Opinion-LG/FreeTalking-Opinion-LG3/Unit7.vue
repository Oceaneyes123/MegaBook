<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/green-pencils-container_23-2147885284.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Get Rid of Final Exams?
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
      <td class = "lowertable" >Final exams should continue to be utilized in schools. First of all, final exams keep students on their toes. In other words, they keep students in check, making sure that they don’t laze around and feel too comfortable when the year’s almost over. Thanks to final exams, students have to keep trying hard in their classes and continue their studies. They won’t just do the bare minimum to pass their classes. In addition, final exams help students to retain the information they learned in class.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >We need to get rid of final exams. If a student has demonstrated their knowledge through quizzes, tests, and homework over the course of a year, then there really is no reason to hand them a 50-page exam. Also, final exams don’t really prepare students for the real world. Most Harvard students don’t take final exams, for example. Out of more than 500 graduate-level courses offered, only 14 had final exams! Plus, what kind of job would ask you to take a multiple-choice exam?</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>comprehensive</b> 포괄적인, 종합적인
        </p>
        <p>
          <b>utilize</b> 활용[이용]하다
        </p>
        <p>
          <b>retain</b> 잊지 않고 있다, 계속 유지하다
        </p>
        <p>
          <b>prepare</b> 준비하다[시키다]
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >기말고사는 학교에서 계속 활용되어야 합니다. 무엇보다도, 기말고사는 학생들을 긴장시킵니다. 다시 말해서, 그들은 한 해가 다 끝났을 때, 게으름을 피우며 너무 편안하게 지내지 않도록 하면 서 학생들을 통제합니다. 기말고사 덕분에 학생들은 수업 시간에 계속해서 열심히 노력하고 공부를 계속해야 합니다. 그들은 수업을 통과하기 위해 단지 겨우 최소의 노력만 기울이지 않을 것입니다. 또한, 기말고사는 학생들이 수업에서 배운 정보를 유지하는 데 도움이 됩니다 </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >기말고사를 없애야 해요. 만약 한 학생이 1년 동안 퀴즈, 시험, 그리고 숙제를 통해 그들의 지식을 증명했다면, 그들에게 50페이지분량의 시험을 제출할 이유가 정말로 없습니다. 또한, 기말고사는 실제로 학생들을 현실 세계에 대비시키지 않습니다. 예를 들어, 대부분의 하버드 학생들은 기말고사를 치르지 않습니다 500 개가 넘는 대학원 과정 중 14개만 최종 시험을 치렀습니다! 또한 어떤 직장에서 여러분에. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Why are final exams given?</li>
          <li>How do you prepare for final exams?</li>
          <li>What does a low final exam result mean?</li>
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
