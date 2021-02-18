<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/serious-employee-attentively-reading-document-focused-thinking-coworking_1163-4108.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Standardized Testing A Good Practice?
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
      <td class = "lowertable" >Richard Phelps, an author, and researcher who has devoted most of his working life to education, says that standardized testing has a positive effect on students. He came to this conclusion after reviewing a century’s worth of studies regarding the benefits of student testing. Phelps also insists that standardized testing is an objective measure of one’s scholastic abilities. Without standardized tests, policymakers would have to analyze tests scored by school teachers. In particular, multiple-choice tests are graded by machines, so they’re not subject to human bias.”</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Standardized tests cannot accurately assess one’s scholastic aptitude. According to Gerald Bracey, an education researcher, standardized tests are unable to measure the following qualities: creativity, critical thinking, resilience, motivation, persistence, curiosity, endurance, reliability, enthusiasm, empathy, self-awareness, self-discipline, leadership, compassion, resourcefulness, honesty, and integrity. Standardized testing forces schools to reduce the time spent on teaching the actual curriculum. Instead of learning valuable life lessons, students are learning how to become good test-takers.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>administer</b> 시행하다
        </p>
        <p>
          <b>objective</b> 객관적인
        </p>
        <p>
          <b>scholastic</b> 학업의
        </p>
        <p>
          <b>aptitude</b> 적성, 능력
        </p>
        <p>
          <b>compassion</b> 연민, 동정심
        </p>
        <p>
          <b>integrity</b> 진실성
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >그의 직장 생활의 대부분을 교육에 바친 작가이자 연구원인 리차드 펠프스는 표준화된 테스트가 학생들에게 긍정적인 영향을 미친다고 말합니다. 그는 학생 시험의 이점에 관한 세기의 가치 연구를 검토한 후에 이 결론에 도달했습니다. 펠프스는 또한 표준화된 시험이 자신의 학력에 대한 객관적인 척도라고 주장합니다. 표준화된 테스트가 없다면 정책 입안자는 학교 교사가 채점한 테스트를 분석해야 할 것입니다 특히 객관식 테스트는 기계에 따라 등급이 매겨지므로 인간의 편견에 영향을 받지 않습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >표준화된 시험은 자신의 학업 적성을 정확하게 평가할 수 없습니다. 교육 연구원인 제랄드 브레이시에 따르면 표준화된 시험은 창의성, 비판적 사고, 탄력성, 동기 부여, 지속성, 호기심, 지구력, 신뢰도, 열정, 공감, 자기 인식, 자기 훈련, 리더십, 연민, 수완, 정직, 그리고 성실성을 측정할 수 없습니다. 표준화된 시험은 학교가 실제 커리큘럼을 가르치는 데 소요되는 시간을 줄이도록 강요합니다. 귀중한 인생 교훈을 배우는 대신, 학생들은 좋은 시험 응시자가 되는 법을 배우고 있습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What can you say about standardized testing? What is its purpose?</li>
          <li>Do you believe that standardized testing effectively measures a student’s scholastic ability?</li>
          <li>Do you agree that preparing for the standardized test makes a student become a good test-taker rather than learning valuable life lessons? Why or why not?</li>
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
