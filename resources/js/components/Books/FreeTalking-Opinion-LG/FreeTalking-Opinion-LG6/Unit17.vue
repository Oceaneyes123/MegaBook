<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/subway-station_1112-1827.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Public Transportation in Seoul Be Free In Case of Severe Pollution?
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
      <td class = "lowertable" >Seoul is full of bad and unhealthy air. Paris recently tried a novel idea toward reducing pollution by making the subway and buses free for a limited time. Seoul should do the same. Lower pollution, fewer sick people, reduced stress and solutions to other problems due to traffic would be worth the cost of operating more subway cars and staff to boost passenger convenience. Of course the free fare system wouldn’t be permanent, but could get more people used to driving to use public transportation more.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Making public transportation free temporarily is not the solution to fight pollution. Look at the crowds during rush hour on the subway and buses. If a no-fare policy takes effect, rush hour would be around the clock. Imagine the crowds of passengers in subway cars packed like sardines in a can. Subway and bus companies are also suffering from large financial deficits. They could raise fares later to make up for their losses. And the main problem with the air in Seoul is pollution from China and smoke from coal-burning factories.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>fare</b> 요금
        </p>
        <p>
          <b>temporarily</b> 일시적인
        </p>
        <p>
          <b>boost</b> 양을 증가시키다
        </p>
        <p>
          <b>permanent</b> 영구적인
        </p>
        <p>
          <b>pack like sardines</b> 빽빽이 들어차다
        </p>
        <p>
          <b>coal</b> 석탄
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >서울은 나쁘고 해로운 공기로 가득 차 있습니다. 파리는 제한된 기간 동안 최근 지하철과 버스를 무상으로 만듦으로써 오염을 줄이는 기발한 생각을 시도하였습니다. 서울도 똑같이 해야 합니다. 더 낮은 오염 수준 그리고, 더 적은 아픈 사람들, 스트레스 감소 그리고 교통으로 인한 다른 문제들의 해결은 승객들의 편의를 증진시키기 위해 더 많은 지하철과 직원들을 운영하는 비용을 지불할 가치가 있습니다. 물론 무상 운임 체계는 영구적이지 않지만, 운전에 익숙한 사람들을 더 많이 대중교통을 사용하도록 할 수 있을 것입니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >대중교통을 일시적으로 무상으로 만드는 것은 공해와 싸울 해결 방안이 아닙니다. 출퇴근시간 동안 지하철과 버스에서의 사람들을 보십시오. 만약 운임을 안 받는 정책이 효력을 발휘하기 시작하면, 출퇴근시간은 24시간 내내 계속될 것입니다. 통조림 캔에 있는 정어리처럼 빽빽이 들어찬 지하철 안에서 있을 승객들을 상상해보세요. 지하철과 버스 회사들은 또한 큰 재정적인 손실을 입게 될 것입니다. 그들은 그들의 손실을 상쇄하기 위하여 후에 운임비를 올릴 것입니다. 서울의 공기의 주요 문제는 중국에서부터 온 공해와 석탄을 태우는 공장에서부터 온 연기입니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Would the free fare system help reduce pollution problems? If yes, how so?</li>
          <li>What do you think would happen to your city if a temporary free fare system takes effect?</li>
          <li>In your opinion, what would be the most effective solution to minimize pollution?</li>
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
