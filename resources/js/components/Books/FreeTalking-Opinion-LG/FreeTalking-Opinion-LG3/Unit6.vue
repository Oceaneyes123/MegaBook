<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/friends-having-fun-while-playing-board-game_155003-11965.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Gambling Be Banned?
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
      <td class = "lowertable" >Gambling is a serious issue that should be banned. Not only is it addictive, but it is also psychologically harmful. The Emotional Neuroscience Center in Massachusetts stated, “Monetary reward in a gambling-like experiment produces brain activation very similar to that observed in a cocaine addict receiving an infusion of cocaine.” Gambling addicts stake more and more money in order to recover what they lost, which is called “chasing losses.” This eventually results in enormous debts, ruining people’s lives in a matter of hours or even seconds.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Gambling is simply a form of leisure, so there is no reason to ban it. People should be allowed to spend their money on recreational activities. Preventing people from spending their money on gambling is a very patronizing thing to do. They know what they’re getting themselves into. In addition, casinos create jobs and contribute to tourism. According to americangaming.org, more than 750,000 people work in casinos across the U.S. The casino industry is a vital part of America’s economy.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>wager</b> (돈을) 걸다
        </p>
        <p>
          <b>neuroscience</b> 신경 과학
        </p>
        <p>
          <b>monetary</b> 통화[화폐]의
        </p>
        <p>
          <b>stake</b> (돈 등을) 걸다
        </p>
        <p>
          <b>debt</b> 빚
        </p>
        <p>
          <b>patronizing</b> 잘난[윗사람인] 체하는
        </p>
        <p>
          <b>vital</b> 필수적인
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >도박은 금지해야 할 심각한 문제입니다. 중독성이 있을 뿐만 아니라 심리적으로도 해롭습니다. 매사추세츠 주의 감성 신경과학센터는 "도박과 유사한 실험에서 금전적인 보상은 코카인 중독자가 코카인을 주입 받는 것을 관찰한 것과 매우 유사한 뇌 활성화를 만들어냅니다."라고 말했습니다. 도박 중독자들은 잃어버린 것을 되찾기 위해 점점 더 많은 돈을 걸게 되는데, 이를 "손실 추적"이라고 합니다. 결국 엄청난 부채가 발생하여 몇 시간 또는 몇 초 안에 사람들의 삶을 망칠 수 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >도박은 단순히 여가의 한 형태이므로 금지 할 이유가 없습니다. 사람들은 그들의 돈을 여가 활동에 쓰도록 허용되어야 합니다. 사람들이 도박에 돈을 쓰는 것을 막는 것은 매우 생색을 내는 일입니다. 그들은 자신들이 어떤 상황에 처하게 될지 알고 있습니다. 또한 카지노는 일자리를 창출하고 관광에 기여합니다 americangaming.org에 따르면, 75만 명 이상의 사람들이 미국 전역의 카지노에서 일하고 있다고 합니다. 카지노 산업은 미국 경제의 중요한 부분입니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Why do people gamble?</li>
          <li>Is gambling legal in your country? If not, why do you think so?</li>
          <li>How can you tell if a person is getting addicted to gambling?</li>
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
