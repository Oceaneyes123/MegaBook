<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/closeup-fingerprint-paper_53876-13400.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Do Electronic Voting Machines Improve The Voting Process?
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
      <td class = "lowertable" >Electronic voting machines make the voting process easier. Disabled voters find them to be quite helpful. According to Jim Dickson, vice president of the American Association of People With Disabilities, “Touchscreens are the only system which allows a voter with a disability to cast a secret and independent vote.” He says features such as audio ballots and adaptive aids are especially helpful. EVMs are also accurate. In 2003, the Touchscreen Task Force said that EVMs eliminate overvotes and undervotes because they provide review screens.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Several countries discontinued electronic voting due to security issues. In 2006, a group in the Netherlands demonstrated security flaws in EVMs, and electronic voting in the country was outlawed a year later. According to the U.S. Government Accountability Office, many EVMs “under examination contained weaknesses in controls designed to protect the system.” In addition, Ireland got rid of electronic voting because of transparency issues. Moreover, EVMs are difficult to use. In 2009, Germany banned EVMs because you need to have the programming knowledge to use them.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>nationwide</b> 전국적으로
        </p>
        <p>
          <b>disabled</b> 장애를 가진
        </p>
        <p>
          <b>accurate</b> 정확한
        </p>
        <p>
          <b>eliminate</b> 없애다
        </p>
        <p>
          <b>outlaw</b> 불법화하다, 금하다
        </p>
        <p>
          <b>transparency</b> 명료성
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >전자 투표 기계는 투표 절차를 보다 쉽게 만듭니다. 장애인 유권자들은 그들이 꽤 도움이 된다고 생각합니다. 미국 장애인 협회 (American Association of Disabilities)의 짐 딕슨 (Jim Dickson) 부회장은 "장애가있는 유권자가 비밀 투표를 할 수 있는 유일한 시스템은 터치 스크린(Touchscreen)뿐입니다. 그는 오디오 투표 용지 및 적응 보조 장치와 같은 기능은 특히 도움이 됩니다.라고 말했습니다. EVM는 또한 정확합니다. 2003년에 터치스크린 태스크 포스(Touchscreen Task Force)는 EVM 검토 화면을 제공하기 때문에 초과 투표와 과소 투표를 제거한다고 말했습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >몇몇 국가에서는 보안 문제로 인해 전자 투표를 중단했습니다. 2006년, 네덜란드(Netherland)의 한 단체가 EVM의 보안상의 결함을 보여주었고, 1년 후 네덜란드의 전자 투표는 불법화되었습니다. 미국 정부 회계감사원에 따르면, 많은 EVM이 "검사 중"시스템을 보호하기 위해 고안된 제어장치의 약점을 포함하고 있었습니다.” 게다가, 아일랜드(Ireland )는 투명성 문제로 인해 전자 투표를 폐지했습니다. 게다가 EVM은 사용하기 어렵습니다. 2009년에 독일은 EVM을 사용하기 위해 프로그래밍 지식이 필요하기 때문에 EVM을 금지했습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you voted before? What would you say to people who haven’t voted yet?</li>
          <li>Which method would make you feel safer and secured? Electronic voting or manual voting?</li>
          <li>Do you believe that voting is important? Why or why not?</li>
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
