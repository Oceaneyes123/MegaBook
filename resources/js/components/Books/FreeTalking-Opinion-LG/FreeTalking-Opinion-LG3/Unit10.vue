<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/front-view-man-young-holding-gun-white-t-shirt-blue-desk_140725-11127.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should People Be Allowed to Carry Concealed Handguns?
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
      <td class = "lowertable" >People should be allowed to carry concealed handguns because they deter crime. According to an analysis of FBI crime data in 2000, states with certain concealed carry laws saw a reduced rate in rapes, murders, assaults, and robberies by 3 to 8.5 percent. Furthermore, a study in Applied Economic Letters found that between 1980 and 2009, “states with more restrictive CCW (carrying concealed weapons) laws had gun-related murder rates that were 10 percent higher.” Also, Larry Craig, a police chief, called concealed weapons a “deterrent.”</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >People should not carry concealed handguns. Public safety should be the responsibility of police officers, not ordinary citizens. Alarmingly, some states, including Georgia and Maryland, do not require any training in order to receive a concealed carry permit. Some states don’t even require a permit at all. In addition, people with concealed weapons make the rest of the public feel unsafe. A recent study showed that 79 percent of college students in the U.S. would not feel safe if concealed weapons were allowed on campus.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>permit</b> 허가증
        </p>
        <p>
          <b>deter</b> 단념시키다, 그만두게 하다
        </p>
        <p>
          <b>murder</b> 살인(죄)
        </p>
        <p>
          <b>restrictive</b> 제한[구속]하는
        </p>
        <p>
          <b>deterrent</b> 제지하는 것
        </p>
        <p>
          <b>ordinary</b> 평범한
        </p>
       
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >이것이 범죄를 그만두게 하기 때문에 은폐된 권총을 휴대하는 것이 허용되어야 합니다. 2000년 FBI 범죄 자료를 분석한 결과, 특정 은폐 휴대법이 있는 주에서는 강간, 살인, 폭행, 강도 발생률이 3~8.5% 감소했습니다. 게다가 Applied Economic Letters의 연구에 따르면 1980년에서 2009년 사이에“더 제한적인 CCW (숨겨진 무기 운반) 법이 있는 주에서는 총 관련 살인율이 10 % 더 높았습니다. 또한, 래리 크레이그 경찰국장은 은폐된 무기를 "단념하게 하는 것"이라고 불렀습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >사람들은 은폐된 권총을 휴대해서는 안 됩니다. 공공 안전은 일반 시민이 아닌 경찰관의 책임이어야 합니다. 놀랍게도, 조지아와 메릴랜드를 포함한 일부 주에서는 은폐된 휴대 허가를 받기 위해 교육이 필요하지 않습니다. 일부 주에서는 전혀 허가가 필요하지 않습니다. 게다가, 은폐된 무기를 가진 사람들은 나머지 대중들을 불안하게 만듭니다. 최근 한 연구에 따르면 미국 대학생의 79%가 은폐된 무기가 캠퍼스에 허용된다면 안전하다고 느끼지 못할 것이라고 합니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are the other forms of self-defense aside from using guns?</li>
          <li>Are you in favor of concealed handguns being allowed in your country? Why or why not?</li>
          <li>Do you think background checks should be strictly implemented before a person is allowed to carry a gun? Why?</li>
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
