<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/dealer-new-cars-stock_1426-1190.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Invest In Self-Driving Cars?
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
      <td class = "lowertable" >Self-driving cars are the wave of the future. 81% of traffic accidents are caused by the driver. If we invested in self-driving cars we would see a remarkable drop in accidents. In addition, self-driving cars would eliminate the problem of drunk drivers. There would even be a remarkable efficiency with self-driving cars, easing congestion and allowing people to get to their destinations sooner. Self-driving cars have sensors which would allow them to drive closer together without hitting each other. With self-driving cars, we could have a world without accidents and quicker commutes.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Self-driving cars are dangerous. While machines are accurate and rarely wrong, there are always moments when GPS tracking and map updates are not made in a timely manner. What if a self-driving car would be instructed to go across a bridge and that bridge was no longer there? In fact, heavy rain is known to cause serious damage to the laser sensors on a self-driving car’s roof. If we all stopped learning how to drive on our own, what would happen if these cars would malfunction? What if the traffic lights stopped working? How would we be able to coordinate the cars then?</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>recent</b> 최근의
        </p>
        <p>
          <b>phenomenon</b> 현상
        </p>
        <p>
          <b>problematic</b> 문제가 있는
        </p>
        <p>
          <b>remarkable</b> 놀랄 만한
        </p>
        <p>
          <b>eliminate</b> 없애다
        </p>
        <p>
          <b>efficiency</b> 효율성, 능률
        </p>
        <p>
          <b>congestion</b> 혼잡
        </p>
        <p>
          <b>commute</b> 통근(거리)
        </p>
        <p>
          <b>accurate</b> 정확한
        </p>
        <p>
          <b>malfunction</b> 오작동
        </p>
          
        
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >자가운전 자동차는 미래의 물결입니다. 81퍼센트의 교통사고는 운전자에 의해 발생합니다. 만약 우리가 자가운전 자동차에 투자한다면, 우리는 사고가 현저하게 줄어드는 것을 볼 것입니다. 게다가, 자가운전 자동차는 음주운전자들의 문제를 제거할 것입니다. 자가운전 자동차가 혼잡을 완화하고 사람들이 그들의 목적지에 더 빨리 도착하게 해 줌에 따라 큰 효율성이 있을 것입니다. 자가운전 자동차들은 서로 부딪히는 일 없이 더 가깝게 운전할 수 있도록 해 주는 센서를 가질 수 있습니다. 자가운전 자동차로, 우리는 사고가 없는 세계를 만들고 더 빠르게 통근할 수 있을 것입니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >자가운전 자동차는 위험합니다. 기계는 정확하고 거의 틀리지 않지만, GPS추적과 지도 업데이트가 적시에 안 이루어지는 순간이 항상 있습니다. 만약 자가운전 자동차가 다리를 건너게 지시받았는데 다리가 더 이상 그곳에 없으면 어떻게 될까요? 사실, 폭우는 자가운전 자동차의 지붕에 있는 레이저 센서에 심각한 손상을 가하는 것으로 알려져 있습니다. 만약 우리 모두가 스스로 운전할 수 있는 방법을 배우는 것을 멈춘다면, 이러한 차들이 오작동할 경우 어떻게 됩니까? 신호등이 더 이상 작동하면 어떻게 됩니까? 우리는 그러면 어떻게 차들을 조율할 수 있겠습니까? </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What do you think of self-driving cars?</li>
          <li>What do you think are the advantages and disadvantages of owning a self-driving car?</li>
          <li>Would you consider having one? Why or why not?</li>
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
