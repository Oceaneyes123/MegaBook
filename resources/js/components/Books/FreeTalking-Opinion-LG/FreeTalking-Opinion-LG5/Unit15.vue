<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/male-hand-answering-questionary-form-with-pen_1262-2288.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Students Be Able To Evaluate Teachers?
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
      <td class = "uppertable" ><b>David :</b></td>
      <td class = "lowertable" >Although self-judgment can be a helpful thing, feedback is necessary for improvement. If a pupil finds things difficult to understand and the teacher cannot explain it properly, the fault is on the teacher. While most assessments are done by superintendents and upper management, these people are rarely around to witness things every day. If students assessed teachers, however, it could provide insight. When a product is being sold, market research is done on the customer. It should be the same for students and their education.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Students, particularly young ones, are bad judges of character. By letting students assess their teachers, we can create a problematic system. Some students might not take it seriously while some teachers may not take students seriously as well. In doing so, both parties lose. In addition, teachers may resort to being liked to get good assessments, much like how a student could pander for good grades. By pandering to students and being lax or giving good grades too easily, the system can only suffer. This system of pandering could end up turning teacher assessments into a farce.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>ancient</b> 고대의
        </p>
        <p>
          <b>pander</b> (남의 약점을) 이용하다
        </p>
        <p>
          <b>fault</b> 잘못, 책임
        </p>
        <p>
          <b>superintendent</b> 관리자, 감독관
        </p>
        <p>
          <b>lax</b> (일, 규칙, 기준 등에 대해) 느슨한[해이한]
        </p>
        <p>
          <b>farce</b> 익살극, 웃음거리
        </p>
         
 
 
 
 
 

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >비록 자가 판단은 도움이 될 수도 있지만, 피드백은 개선에 필수적입니다. 학생이 이해하기 어려운데 교사가 그것을 적절하게 설명할 수 없다면, 잘못은 교사에게 있습니다. 대부분의 평가가 관리자와 고위 경영진에 의해 이뤄지는 반면, 이 사람들은 거의 매일 일어나는 일들을 보는 자리에 없습니다. 그러나 학생들이 교사들을 평가할 수 있다면, 그것은 통찰력을 줄 수 있을 것입니다. 제품이 팔리면, 시장 조사는 고객에 대하여 시행됩니다. 학생들과 그들의 교육에 대해서도 똑같은 일이 행해져야 합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >학생들, 특히 어린 학생들은 성격을 잘 판단하지 못합니다. 학생들이 그들의 선생님들을 평가하게 함으로써, 우리는 문제가 있는 제도를 만들 수 있습니다. 일부 학생들은 그것을 진지하게 받아들이지 않을 수도 있는 반면 일부 선생님들도 학생들을 진지하게 받아들이지 않을 수도 있습니다. 그렇게 함으로써, 양쪽 다 손해를 봅니다. 게다가, 학생이 좋은 성적을 위해 상황을 이용하는 것처럼, 선생님들도 좋은 성적을 얻기 위해 인기를 얻는 것에 의존할 수 있습니다. 학생들에게 영합하고 느슨해지거나 좋은 성적은 너무 쉽게 주듯이, 그 제도는 단지 악화될 수 있습니다. 이 영합하는 제도는 교사 평가를 웃음거리로 바꾸는 것으로 끝날 수 있습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you experienced evaluating the performance of someone who has a higher position than you? If yes, how was it?</li>
          <li>What are your thoughts on students evaluating their teachers?</li>
          <li>Do you think students could also be good judges of character? Why or why not?</li>
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
