<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/mugs-with-marshmallows-near-warm-wear_23-2147967465.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Staying Warm in the Winter
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
      <td class = "lowertable" >Instead of turning up the heater, you should rely on alternative methods. Warming tents are inexpensive, costing around W30,000 on most online shops. They may seem like ordinary camping tents, but once you go inside one, you can actually feel a difference in the temperature. Most warming tents guarantee an increase of 5 to 10 degrees Celsius. In addition, wear multiple layers of clothes when you’re awake and doing menial tasks. In general, stay away from anything that requires the use of electricity or gas.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Although heating bills can sometimes be a burden, there are ways to use the heater more efficiently. Many people turn up the heater way too high. The ideal home temperature, according to energystar.gov, is between 21 to 25 degrees Celsius. It is tempting to raise the temperature very high so that you can feel immediate warmth during the winter, but you must be patient. Set your heater to 23 degrees, for example, and take advantage of its power-saving features. Electric blankets and mini heaters are also very effective.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>ordinary</b> 보통의, 평범한
        </p>
        <p>
          <b>menial</b> 하찮은
        </p>
        <p>
          <b>efficiently</b> 효율적으로
        </p>
        <p>
          <b>tempting</b> 솔깃한, 구미가 당기는
        </p>
        <p>
          <b>immediate</b> 즉각적인
        </p>
        <p>
          <b>patient</b> 참을성 있는
        </p>
    
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >히터를 켜는 대신 다른 방법을 사용해야 합니다. 난방텐트는 대부분의 온라인 상점에서 약 3만원 정도로 저렴합니다. 평범한 캠핑 텐트처럼 보일지 모르지만 일단 들어가면 실제로 온도의 차이를 느낄 수 있습니다. 대부분의 난방텐트는 섭씨 5~10 도의 상승을 보장합니다. 게다가, 여러분이 깨어 있을 때 그리고 소일거리를 할 때 여러 겹의 옷을 입으세요. 일반적으로 전기나 가스의 사용을 필요로 하는 모든 것을 멀리 하세요.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >난방비가 때때로 부담이 될 수 있지만 히터를 더 효율적으로 사용할 수 있는 방법이 있습니다. 많은 사람들이 히터를 너무 높게 설정합니다 energystar.gov에 따르면 이상적인 가정 온도는 섭씨 21도에서 25도 사이라고 합니다. 겨울에 즉각적인 따뜻함을 느낄 수 있도록 온도를 매우 높이고 싶지만 인내심이 있어야 합니다. 예를 들어 히터를 23도로 설정하고 절전 기능을 활용하십시오 전기 담요와 미니 히터도 매우 효과적입니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like winter? Why or why not?</li>
          <li>What do you usually do to keep yourself or your house warm during winter?</li>
          <li>Do you think it’s more practical to use warming tents instead of heaters? Why?</li>
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
