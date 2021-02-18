<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/inside-view-train-stopped-with-open-door_23-2148139932.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is It Better to Take a Car Than the Subway?
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
      <td class = "lowertable" >When it comes to transportation, nothing beats taking the car. While the subway can be jam-packed with people, cars are your property. This means that you have more privacy and space, creating a more relaxed and comfortable ride to your destination. When you take the subway, you have to deal with people who are impatient, frustrated, and stressed from all sorts of factors. There’s even a condition called commute stress. According to researchers at McGill University, nearly every commuter who has taken public transit has experienced stress.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >We should try to take the subway as much as possible. According to The Times, cars are the biggest cause of greenhouse gases, which contribute to global warming. Many people are trying to use less plastic these days, but we should also try to use the subway more. In addition, there’s too much traffic. You’ll help ease traffic congestion by taking the subway. Finally, subways are safer than cars. Every year, around 40,000 people around the world die from car accidents.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>jam-packed</b> 빽빽히 찬
        </p>
        <p>
          <b>property</b> 재산, 소유물
        </p>
        <p>
          <b>impatient</b> 성급한, 참을성 없는
        </p>
        <p>
          <b>commute</b> 통근
        </p>
        <p>
          <b>contribute</b> 한 원인이 되다
        </p>
        <p>
          <b>congestion</b> 혼잡
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >교통수단에 관한 한, 차를 타는 것보다 더 좋은 것은 없습니다. 지하철은 사람들로 꽉 찰 수 있지만, 자동차는 여러분의 소유물입니다. 이것은 여러분이 더 많은 사생활과 공간을 가지고 있다는 것을 의미하며, 여러분의 목적지까지 더 편안하고 안락하게 탈 수 있게 해줍니다 지하철을 탈 때, 여러분은 초조하고, 좌절하고, 온갖 요인들로 스트레스를 받는 사람들을 상대해야 합니다. 심지어 통근 스트레스라는 현상도 있습니다. 맥길 대학의 연구원들에 따르면, 대중교통을 이용하는 거의 모든 통근자들이 스트레스를 경험했다고 합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >우리는 가능한 한 지하철을 타도록 노력해야 합니다. 더 타임즈에 따르면, 자동차는 지구 온난화에 기여하는 온실 가스의 가장 큰 원인이라고 합니다. 요즘 많은 사람들이 플라스틱을 덜 쓰려고 하지만, 우리는 지하철을 더 많이 이용하도록 노력해야 합니다. 게다가 교통량이 너무 많습니다. 지하철을 타면 교통 혼잡을 완화하는데 도움이 됩니다 마지막으로, 지하철은 자동차보다 안전합니다. 매년, 전세계 약 4만 명의 사람들이 자동차 사고로 사망합니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you own a car? If yes,  would you prefer taking it rather than the subway? Why or why not?</li>
          <li>What risks does taking the subway impose?</li>
          <li>Which travel experience is better? Taking the car or subway? Why?</li>
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
