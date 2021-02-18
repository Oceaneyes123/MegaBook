
<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://images.pexels.com/photos/2363/france-landmark-lights-night.jpg?auto=compress&cs=tinysrgb&h=750&w=1260" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Museums Charge Money?
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
      <td class = "lowertable" >Museums are already charging money, and some of the best ones in the world have maintained a high standard as a result of this. The Louvre charges for admission, and has the greatest collection the world has ever seen. By charging admission, they can maintain the facility and continue to invest in artwork that will only make the museum more popular. Other museums, like the Guggenheim, have a yearly membership which allows members to visit and take part in member-only activities, giving them the chance to take part in how the museum is run.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >When money gets involved with education, only bad things can happen. The Metropolitan Museum of Art had financial backing of several trustees which created a disproportionate salary for many executives at the museum. Some had been given compensation of a million dollars with bonuses of a hundred thousand, something that is unheard of in museums. These setbacks have caused a great decline in the quality of purchasing exhibits. As a result, the growing debt forced a postponement in purchase of several pieces of art, and the expansion of the museum. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>facility</b> 시설
        </p>
        <p>
          <b>yearly</b> 1 년에 한 번씩 있는
        </p>
        <p>
          <b>back</b> 도와주다
        </p>
        <p>
          <b>trustee</b> 신탁 관리자
        </p>
        <p>
          <b>disproportionate</b> 균형이 안 맞는
        </p>
        <p>
          <b>executive</b> 경영 간부
        </p>
        <p>
          <b>compensation</b> 보상, 이득
        </p>
        <p>
          <b>unheard</b> 아무도 귀 기울이지 않는
        </p>
        <p>
          <b>setback</b> 차질
        </p>
        <p>
          <b>postponement</b> 연기
        </p>
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >박물관들은 이미 돈을 받고 있으며 세계에서 최고의 박물관들 중 몇몇은 그로 인해 높은 수준을 유지하고 있습니다. 루브르 박물관은 입장을 위해 돈을 부과하고, 세계가 목격한 가장 위대한 전시물을 가지고 있습니다. 입장료를 받음으로써, 그들은 그 시설을 유지할 수 있고, 박물관을 더 유명하게 할 예술품들에 투자를 계속할 수 있습니다. 구겐하임과 같은 다른 박물관들은 멤버들이 방문하고 멤버들에게만 제한되는 활동들에 참여하도록 허용하는 연례 회원권을 가지고 있는데, 이것은 그들이 어떻게 박물관이 운영되는지에 대해 참여할 수 있는 기회를 제공합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >돈이 교육에 수반될 때 나쁜 일만 일어날 뿐입니다. 뉴욕 메트로폴리탄미술관은 박물관의 많은 간부들 간 균형이 맞지 않는 급여를 만든 몇몇 신탁 관리자들의 재정적인 지원을 받고 있습니다. 몇몇은 십 만 달러의 보너스와 백 만 달러의 보상금을 받았는데, 이것은 박물관 내에 있어 전례가 없는 일입니다. 이러한 차질들은 전시물을 구매하는 질에 엄청난 감소를 가져왔습니다. 결과적으로, 점점 채무가 증가하면서 몇몇 예술 작품들의 구매와 박물관 확장을 연기할 수밖에 없도록 하였습니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you been to a museum? If yes, what kind of museum did you visit? </li>
          <li>What do you think are museums for?</li>
          <li>Do you think it is right for museums to charge money? Why or why not</li>
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
