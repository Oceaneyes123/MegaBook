<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/hands-young-man-handcuffs_144627-21856.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should the Death Penalty Be Allowed?
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
      <td class = "lowertable" >Many people believe that punishing a criminal with death is immoral. However, the death penalty is given to the worst of the worst. According to Edward Feser, a philosophy professor at Pasadena City College, and Joseph Bessette, an ethics professor at Claremont McKenna College, the capital punishment system is not a “lottery that randomly chooses an unlucky few for the ultimate penalty.” They said that anything “less than death would fail to do justice because the penalty would be disproportionate to the heinousness of the crime.”</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >According to John J. Donohue, a law professor at Stanford University, there aren’t any credible statistics that show that the death penalty reduces the homicide rate. He compared statistics from the U.S., Canada, Hong Kong, Singapore, and several other countries to come to the conclusion that “there is no detectable effect of capital punishment on crime.” Donohue said, “The likelihood is incredibly remote that some small chance of execution many years after committing a crime will influence the behavior of a sociopathic deviant.”</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>deter</b> 그만두게 하다
        </p>
        <p>
          <b>financial</b> 금융[재정]의
        </p>
        <p>
          <b>perpetuate</b> 영구화하다, 영속시키다
        </p>
        <p>
          <b>immoral</b> 비도덕적인
        </p>
        <p>
          <b>ethics</b> 윤리학
        </p>
        <p>
          <b>disproportionate</b> 불균형의
        </p>
        <p>
          <b>heinousness</b> 극악[흉악]함
        </p>
        <p>
          <b>homicide</b> 살인
        </p>
        <p>
          <b>sociopathic</b> 반사회적인
        </p>
        <p>
          <b>deviant</b> 사회의 상식에서 벗어난 사람
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >많은 사람들은 죽음으로 범죄자를 처벌하는 것이 부도덕하다고 생각합니다. 하지만, 사형은 최악의 경우에 주어집니다. 패서디나 시티 칼리지의 철학 교수인 에드워드 페서와 클레어몬트 맥케나 칼리지의 윤리학 교수 인 조셉 베셋에 따르면, 사형제도는“최종적인 처벌을 위해 불운한 극소수를 무작위로 선택하는 추첨"이 아니라고 합니다. 그들은 "사망 이하의 것은 죄질이 극악무도한 것과 불균형하기 때문에 정의를 행하지 못할 것이다"라고 말했습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >스탠퍼드대 법학과 존 J. 도노휴 교수에 따르면, 사형이 살인률을 감소시킨다는 믿을 만한 통계가 없다고 합니다. 미국, 캐나다, 홍콩, 싱가포르 등 여러 나라의 통계를 비교해 "범죄에 대한 사형의 감지 가능한 효과는 없다"는 결론을 내렸습니다. 도노휴는 "범죄를 저지르고 수년 후에 처형될 작은 가능성이 반사회적 일탈자의 행동에 영향을 미칠 가능성은 매우 희박하다 가능성이 매우 희박하다"고 말했습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Why do you think was the death penalty created?</li>
          <li>Is death penalty being implemented in your country? Are you in favor of this policy? Why or why not?</li>
          <li>Why are many people against death penalty?</li>
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
