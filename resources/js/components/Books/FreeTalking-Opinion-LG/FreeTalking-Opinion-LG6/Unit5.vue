<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/career-elementary-discover-tie-cute_1134-1267.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Keep Letter Grades?
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
      <td class = "lowertable" >Grades have been around since public education began. Without grades we cannot properly assess a student and give them the clear feedback they require. In addition, being able to see tangible results provides the motivation to keep going. It lets a student know what their strengths and weaknesses are, and in doing so can provide guidance for where improvement may be necessary as well as where their future strengths should be concentrated.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Grades may be good for showing feedback, but they are often very subjective. In one math class a teacher might assign more points for showing your work instead of just answering the question. Moreover, grades are not motivation to actually learn and better oneself, but to memorize facts according to how a teacher would assess things. In addition, studies show that a high number of teachers often grade tests better after taking a break from grading, showing just how subjective grading is.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>subjective</b> 주관적인
        </p>
        <p>
          <b>tangible</b> 분명히 실재하는, 유형의
        </p>
        <p>
          <b>feedback</b> 피드백
        </p>
        <p>
          <b>motivation</b> [심리] (행동의) 동기 부여, 학습 의욕 유발
        </p>
        <p>
          <b>assess</b> (특성·자질 등을) 재다[가늠하다]
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >성적은 공교육이 시작된 이래로 있어 왔습니다. 성적 없이 우리는 적절히 학생들을 평가할 수 없고 그들이 필요로 하는 분명한 피드백을 제공할 수 없습니다. 게다가, 가시적인 결과를 볼 수 있는 것은 계속 할 동기 부여를 제공해 줍니다. 그것은 학생들이 그들의 장점과 약점이 무엇인지 알게 해 주고, 그렇게 함으로써 미래의 장점이 어디에 집중되어야 되는지 뿐만 아니라 어디의 개선이 필요한지에 대해 지도해 줍니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >성적은 피드백을 보여주는 데 좋을 수 있지만, 그것들은 자주 주관적입니다. 한 수학 교실에서 선생님은 단순히 답을 맞추는 것 대신 그들의 숙제를 보여주는 것에 더 많은 점수를 할애할지도 모릅니다. 더욱이, 성적은 실제로 배우고 자기 자신을 진보시키는 것이 아니라, 선생님이 평가하는 방식에 따라 사실들을 암기하는 동기 부여입니다. 게다가, 많은 연구는 많은 선생님들이 자주 점수를 매기는 것으로부터 휴식을 취한 후에 더 성적을 잘 처리한다고 보여왔으며, 이는 성적이 얼마나 주관적인지 보여줍니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What do you think of letter grades?</li>
          <li>Do you agree that grades are important? Why or why not?</li>
          <li>Do you believe that grades help motivate a student?</li>
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
