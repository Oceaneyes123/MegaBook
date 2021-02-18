<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://www.jayshreetea.com/wp/wp-content/uploads/2019/04/Tea-Vs-Coffee.png" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Tea Healthier Than Coffee?
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
      <td class = "lowertable" >Many people drink coffee to feel more alert, but this is because their bodies depend on caffeine. According to researchers from the University of Bristol, coffee drinkers suffer from withdrawal symptoms and need caffeine to be productive. According to a study in Frontiers in Bioscience, drinking tea “can help to protect neurons” and “reduce the decline in brain function.” The study’s lead researcher explained that tea has amino acids that “have benefits for memory and reduce the decline in cognitive function as we get older.”.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >If you want to live a longer life, then you should be drinking coffee. According to a study in the New England Journal of Medicine, people who drink six or more cups of coffee per day have a 10 to 15 percent lower risk of death compared to those who do not. In addition, coffee is great for heart health. A Dutch research paper published in the Journal of the American Heart Association says that coffee drinkers have a 20 percent lower risk of heart disease.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>alert</b> 기민한, 정신이 초롱초롱한
        </p>
        <p>
          <b>withdrawal</b> 금단
        </p>
        <p>
          <b>productive</b> 생산적인
        </p>
        <p>
          <b>amino acid</b> 아미노산
        </p>
        <p>
          <b>cognitive</b> 인지의
        </p>
        <p>
          <b>function</b> 기능
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >많은 사람들이 더 긴장감을 느끼기 위해 커피를 마시지만, 이것은 그들의 신체가 카페인에 의존하기 때문입니다 브리스톨(Bristol) 대학의 연구원들에 따르면, 커피를 마시는 사람들은 금단 증상으로 고생하고 있으며,생산적으로 되기 위해서 카페인이 필요하다고 합니다. 생명 공학 분야의 프론티어 (Frontiers in Bioscience)연구에 따르면 차를 마시는 것은 "신경세포를 보호하는 데 도움이 될 수 있습니다"그리고 "뇌 기능 저하를 감소시킬 수 있습니다." 이 연구의 수석 연구원은 차에는 "우리가 나이가 들수록 기억력에 이로운 점이 있고 인지 기능의 쇠퇴를 줄이는 아미노산(amino acid)이 있다”라고 설명했습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >만약 여러분이 더 오래 살고 싶다면, 커피를 마셔야 합니다. 뉴 잉글랜드 의학 저널 (New England Journal of Medicine)의 한 연구에 따르면 하루 6 잔 이상의 커피를 마시는 사람들은 그렇지 않은 사람들에 비해 사망 위험이 10-15 % 낮습니다 또한 커피는 심장 건강에 좋습니다. 미국 심장 협회(American Heart Association )저널에 실린 네덜란드(Dutch) 연구 논문에 따르면 커피를 마시는 사람은 심장 질환 위험이 20 % 낮습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What do you usually drink? Tea or coffee? Why?</li>
          <li>How often do you drink these kinds of beverages?</li>
          <li>Between tea and coffee, which drink do you think has more health benefits?</li>
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
