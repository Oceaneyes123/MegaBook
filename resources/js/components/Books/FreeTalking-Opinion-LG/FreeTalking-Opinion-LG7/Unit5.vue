<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/mother-assisting-daughter-washing-plate-kitchen_1170-2831.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Dishwashers Versus Dishwashing
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
      <td class = "lowertable" >We should start relying on electric dishwashers. According to a study in the journal Environmental Research Communications, using a dishwasher is actually better for the environment than using traditional washing techniques. Traditional dishwashing uses 34,200 gallons of water in a span of 10 years. Compare that to electric dishwashers, which use an average of only 16,300 gallons. Plus, compared with dishwashers, traditional dishwashing produces more than double the amount of greenhouse gas emissions. Why wash the dishes yourself? Saving up for a dishwasher is definitely worth it!</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Dishwashers aren’t very good at making everything spotless and pristine. Getting rid of all the grime requires intense scrubbing from a pair of hands. Moreover, there are things you can and cannot throw into the dishwasher. Aluminum, ashtrays, blenders, wine glasses, plastic, sharp knives, non-stick pans, fine china, and Thermos bottles are some of the many items that should be washed by hand. In addition, dishwashers require constant cleaning. Otherwise, they’ll get moldy and leave stains. Save your money and wash your dishes by hand, even if it’s a chore!</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>save up</b> (돈을) 모으다
        </p>
        <p>
          <b>pristine</b> 아주 깨끗한
        </p>
        <p>
          <b>grime</b> 때
        </p>
        <p>
          <b>scrub</b> (보통 비눗물과 솔로) 문질러 씻다
        </p>
        <p>
          <b>ashtray</b> 재떨이
        </p>
        <p>
          <b>Thermos bottle</b> 보온병
        </p>
        <p>
          <b>moldy</b> 곰팡이가 핀
        </p>
        <p>
          <b>stain</b> (지우기 힘든) 얼룩
        </p>
        <p>
          <b>chore</b> 하기 싫은[따분한] 일
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >우리는 전기 식기 세척기에 의존하는 것을 시작해야 합니다. 학술지 환경연구통신에 실린 한 연구에 따르면, 식기세척기를 사용하는 것이 전통적인 설거지를 하는 것보다 실제로 환경에 더 좋다고 합니다. 전통적인 설거지는 10년 동안 34,200갤런의 물을 사용합니다.. 평균 16,300갤런밖에 사용하지 않는 전기 식기 세척기와 비교해 보세요. 게다가, 식기 세척기와 비교했을 때, 전통적인 설거지는 온실 가스 배출량의 두 배 이상을 생산합니다. 왜 직접 설거지를 하나요? 식기세척기를 위해 돈을 모우는 것은 분명히 가치가 있습니다!</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >식기세척기는 모든 것을 티끌 하나 없이 아주 깨끗하게 만드는데 그다지 좋지 않습니다. 모든 얼룩을 없애려면 양손으로 강하게 문질러야 합니다. 또한 식기 세척기에 넣을 수 있는 것과 넣을 수 없는 것이 있습니다. 알루미늄, 재떨이, 블렌더, 와인잔, 플라스틱, 날카로운 칼, 넌 스틱 팬, 고급 도자기, 보온병은 손으로 씻어야 할 많은 품목 중 일부입니다. 또한 식기 세척기는 지속적인 세척이 필요합니다. 그렇지 않으면 곰팡이가 생기고 얼룩이 남습니다. 비록 그것이 귀찮더라도, 돈을 절약하고 손으로 설거지를 하세요!</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you wash the dishes? If yes, how often?</li>
          <li>Have you ever tried using a dishwasher? How was it?</li>
          <li>For you, is there any advantage in dishwashing manually over dishwashers?</li>
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
