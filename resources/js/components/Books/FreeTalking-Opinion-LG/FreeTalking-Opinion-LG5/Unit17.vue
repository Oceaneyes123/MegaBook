<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/security-guard-frisk-passengers-standing-queue_107420-85133.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Airport Security Be As Invasive?
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
      <td class = "lowertable" >When you go through airport security they must ensure that passengers are just passengers. After 9/11 and the number of hijacking attempts, security was enhanced to ensure the safety of all. And while it has become more invasive, with body scans and restrictions of liquids, it has been successful. Since 2010, the number of airplane hijackings has been cut in half. While many can argue that it is because the war on terror has become more centralized in the Middle East, many point to the effectiveness of airport security. Despite the discomfort of screening, passengers will walk into the flight safe and secure.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Airport security doesn’t have to be as invasive and fear inducing, but it is. If people opt to take a pat-down instead of the x-ray scanner the personnel are instructed to be as thorough as possible. In the TSA (U.S Transportation Security Administration) manual, the pat-down instructions are to “involve the use of the fingers and palm to search for concealed items and more detailed tactile inspection of areas higher on the thigh, in the groin area, and chest.” This extreme invasion of privacy is extremely unnecessary. What is worse is that those with prosthetics or pacemakers will have no choice but to get the pat-down.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>racism</b> 인종 차별 행위
        </p>
        <p>
          <b>hijacking</b> 공중 납치, 강탈
        </p>
        <p>
          <b>attempt</b> (특히 힘든 일에 대한) 시도
        </p>
        <p>
          <b>restriction</b> 제한, 규제
        </p>
        <p>
          <b>centralize</b> ~에 집중시키다
        </p>
        <p>
          <b>discomfort</b> (심리적) 불편
        </p>
        <p>
          <b>pat-down</b> (옷 위로 더듬어 하는) 몸수색
        </p>
        <p>
          <b>conceal</b> 숨기다
        </p>
        <p>
          <b>tactile</b> 촉각으로 알 수 있는
        </p>
        <p>
          <b>prosthetics</b> 인공 삽입물들
        </p>
     
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >당신이 공안 검문소를 거칠 때 그들은 승객들이 단지 승객이라는 것을 보장해야만 합니다. 9.11과 여러 공중 납치 시도들 이후, 보안은 모두의 안전을 보장하기 위해 강화되었습니다. 신체 스캔과 액체물 제한으로 더 침해가 되었지만, 그것은 성공적이었습니다. 2010년 이래로, 비행기 강탈 사례의 수는 반으로 줄었습니다. 많은 이들이 테러에 대한 전쟁이 중동에 더 집중되었기 때문이라고 주장할 수 있지만, 많은 이들은 공항 검문소의 효과성을 주목합니다. 검사의 불편함에도 불구하고, 승객들은 안전하고 확실하게 비행할 수 있을 것입니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >공항 검문소는 그렇게 침해를 하고 두려움을 유도할 필요가 없지만 그렇습니다. 사람들이 엑스레이 스캔 대신 몸 수색을 선택한다면 직원은 가능한 철저하도록 지도를 받습니다. 미국 교통안전청(TSA)의 매뉴얼에서는 몸 수색 지시가 “숨겨진 물건을 찾기 위해 손가락과 손바닥의 사용과 허벅지 위 부분들과, 사타구니 부분 그리고 가슴의 세부적인 촉각을 이용한 검사를 수반한다”입니다. 이러한 사생활의 극단적인 침입은 극도로 불필요합니다. 설상가상은 인공 삽입물과 심박 조율기를 가진 사람들이 몸수색을 받아야 한다는 것입니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you find airport securities to be invasive? Why or why not?</li>
          <li>Why do you think airport securities should be as thorough as possible?</li>
          <li>What are your thoughts on pat-down inspections?</li>
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
