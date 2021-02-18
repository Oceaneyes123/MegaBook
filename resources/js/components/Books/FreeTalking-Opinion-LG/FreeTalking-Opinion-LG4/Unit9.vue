<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/candid-shot-emotional-ecstatic-teenage-boy-with-braces-sitting-couch-with-his-little-brother-using-laptop-computer-shouting-pumping-fists-rejoicing-his-winning-video-game_343059-168.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Do Violent Video Games Contribute To Youth Violence?
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
      <td class = "lowertable" >Playing violent video games has been proven to cause aggression among children. According to psychologist Lawrence Kutner, children who play violent video games are more likely to hit people. In addition, a study in the Journal of the American Medical Association says that students are more likely to bully others, get into fights, and argue with teachers if they play violent video games regularly. Plus, we all know that children have trouble separating fantasy from reality and end up imitating violent video game characters.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Many children relieve stress by playing violent video games, leading to less aggression. According to a study in the Journal of Adolescent Health, about 60 percent of children play video games because doing so helps them to relax. Around 45 percent say video games help them get their anger out, and nearly 50 percent say they help them forget their problems. And according to researcher Matthew Grizzard, playing violent video games induces a feeling of guilt that leads to increased prosocial behavior and moral sensitivity.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>minority</b> 소수집단
        </p>
        <p>
          <b>aggression</b> 공격성
        </p>
        <p>
          <b>imitate</b> 흉내내다
        </p>
        <p>
          <b>guilt</b> 죄책감
        </p>
        <p>
          <b>prosocial</b> 친사회적인
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >폭력적인 비디오 게임을 하는 것은 어린이들 사이에 공격성을 일으키는 것으로 입증되었습니다. 심리학자 인 로렌스 커트너 (Lawrence Kutner)에 따르면 폭력적인 비디오 게임을 하는 어린이는 사람들을 때릴 가능성이 더 크다고 합니다. 또한 미국 의학 협회 (American Medical Association) 지에 발표 된 한 연구에 따르면 학생들은 폭력적인 비디오 게임을 정기적으로 하는 학생들이 다른 학생들을 괴롭히거나 싸우거나 교사들과 논쟁 할 가능성이 더 많다고 합니다. 게다가 우리는 아이들이 현실과 환상을 분리하는 데 어려움을 겪고 결국 폭력적인 비디오 게임 캐릭터를 모방하는 것을 알고 있습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >많은 어린이들이 폭력적인 비디오 게임을 함으로써 스트레스를 해소하고 공격성을 감소시킵니다. 청소년 건강 저널(Journal of Adolescent Health)의 연구에 따르면, 약 60 퍼센트의 어린이들이 휴식을 취하는데 도움이 되기 때문에 비디오 게임을 한다고 합니다. 약 45 %는 비디오 게임이 노여움을 낫게 하는 데 도움이 된다고 응답했으며 약 50 %는 비디오 게임을 통해 자신의 문제를 잊어 버리는데 도움을 준다고 응답했습니다. 그리고 연구원 매튜 그리자드(Matthew Grizzard)에 따르면 폭력적인 비디오 게임을 하는 것은 친사회적 행동과 도덕적 감수성을 증가시키는 죄책감을 유발한다고 합니다 </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you play computer games? If yes, what computer games do you usually play?</li>
          <li>What can you say about violent games? Do you think it's appropriate for kids to play them? Why or why not?</li>
          <li>In your opinion, do you think playing violent video games help relieve stress?</li>
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
