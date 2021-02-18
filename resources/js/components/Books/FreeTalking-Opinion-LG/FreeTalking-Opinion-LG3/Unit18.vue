<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/breakfast-platter-with-mixed-combination-foods_114579-2109.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Eat Breakfast?
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
      <td class = "lowertable" >According to the Association of U.K. Dieticians, two out of three British adults eat breakfast regularly. According to The American Journal of Clinical Nutrition, one out of four American adults tend to skip breakfast. These are alarming facts. Dietician Sarah Elder says, “The body uses a lot of energy for growth and repair through the night. Eating a balanced breakfast helps to up our energy as well as protein and calcium used throughout the night.” Basically, eating breakfast helps to break our overnight fast.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >A lot of people believe that if you skip breakfast, you’ll binge and eat more than what is necessary later throughout the day. However, a study published in the British Medical Journal found that people who eat breakfast consume significantly more calories than those who skip it, and they end up weighing more. Specifically, those who skipped breakfast ate an average of 260 fewer calories a day. The researchers wrote, “Caution is needed when recommending breakfast for weight loss, as it could have the opposite effect.”</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>substantial</b> 상당한
        </p>
        <p>
          <b>skip</b> 거르다
        </p>
        <p>
          <b>alarming</b> 걱정스러운
        </p>
        <p>
          <b>fast</b> 단식
        </p>
        <p>
          <b>binge</b> 폭식하다
        </p>
        <p>
          <b>caution</b> 조심
        </p>
        <p>
          <b>opposite</b> 반대의
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >영국 영양사 협회에 따르면, 영국 성인 3명 중 2명은 정기적으로 아침을 먹는다고 합니다. 미국 임상 영양학 저널(The American Journal of Clinical Nuture)에 따르면, 미국 성인 4명 중 1명은 아침을 거르는 경향이 있다고 합니다. 이것들은 놀라운 사실들입니다. 영양사 사라 엘더(Sarah Elder)는 "몸은 밤새 성장과 회복을 위해 많은 에너지를 사용합니다. 균형 잡힌 아침식사를 먹는 것은 밤새 사용되는 단백질과 칼슘뿐만 아니라 에너지 증가에 도움이 됩니다." 라고 말합니다. 기본적으로, 아침을 먹는 것은 밤사이 금식을 깨는 데 도움이 됩니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >많은 사람들은 아침을 거르면 나중에 하루 종일 필요한 것보다 더 많이 먹고 폭식을 할 것이라고 믿고 있습니다. 하지만 영국 의학 저널에 발표된 한 연구에 따르면 아침을 먹는 사람들은 아침을 거르는 사람들보다 칼로리가 훨씬 더 많이 소비되고, 결국 체중이 더 많이 나가는 것으로 나타났습니다. 구체적으로, 아침을 거른 사람들은 하루에 평균 260칼로리를 덜 먹었습니다. 연구팀은 "체중 감소를 위해 아침식사를 권할 때 반대 효과가 있을 수 있어 주의가 필요하다"고 썼습니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you usually eat breakfast? What breakfast meals are your favorites?</li>
          <li>Have you tried skipping breakfast? How did it affect you?</li>
          <li>Do you believe that breakfast is the most important meal of the day? Why or why not?</li>
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
