<template>

    <div :style = "{fontSize: fontSize + 'px'}">
  
      <v-container fluid ma-0 pa-0>
  
        <v-layout column>
          <v-img src="https://marketplace.canva.com/MADQ4zHadxQ/1/screen_2x/canva-kids-riding-the-school-bus-MADQ4zHadxQ.jpg" style="max-width: 100%; display:block; height: auto;">
  
          <v-layout
          align-end
          fill-height
          pa-0
          white--text
          >
  
          <transition name="slide-fade">
          <h1 v-if="showTitle" class = "upper-header-lg">Is It Okay for Students to Drop Out of School?
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
        <td class = "lowertable" >Students should be allowed to decide whether they should drop out of school. There are many circumstances as to why someone would drop out. Plus, dropping out of school doesn’t mean you’re abandoning your studies. For example, a student who is constantly bullied may decide to drop out and continue their education online or get homeschooled. Transferring to a different school may not be effective. According to The Research Alliance for New York City Schools, learning environments play a significant role in a student’s success.</td>
      </tr>
      <tr class = "second-dialog-lg">
        <td class = "uppertable" ><b>Ashley :</b></td>
        <td class = "lowertable" >Students should not be allowed to drop out of school. First of all, students between the ages of nine and 18 who dropout of school get a monthly subsidy of W200,000 in Seoul. Although the goal of this policy is to encourage students to buy books and take online courses, the money might be used for other purposes. Maybe they’ll use this money to buy video games, snacks, clothes, or something illegal. If you take this into consideration, these subsidies are a complete waste of tax money.</td>
      </tr>
  
      </table>
  
        <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Vocabulary</h3>
  
        <div style="padding : 16px;">
  
          <p>
            <b>circumstance</b> 사정, 상황
          </p>
          <p>
            <b>abandon</b> 포기하다
          </p>
          <p>
            <b>constantly</b> 끊임없이
          </p>
          <p>
            <b>transfer</b> 전학 가다
          </p>
          <p>
            <b>subsidy</b> 보조금
          </p>
          <p>
            <b>purpose</b> (특정 상황에서 무엇을) 하기 위함, 용도
          </p>
          <p>
            <b>waste</b> 낭비하다
          </p>
  
        </div>
  
        <div class ="line-lg">
        </div>
        <h3 class = "border-translate-lg white--text">해석</h3>
  
        <div style="padding : 16px;">
  
          <table class = "standard-table">
  
            <tr>
              <td class = "uppertable" ><b>Henry :</b></td>
              <td class = "lowertable" >학생들은 그들이 학교를 중퇴해야 하는지 여부를 결정할 수 있어야 합니다. 누군가가 왜 자퇴하는지에 대해서는 여러 가지 사정이 있습니다. 게다가, 학교를 중퇴한다고 해서 학업을 포기하는 것은 아닙니다. 예를 들어, 지속적으로 괴롭힘을 당하는 학생은 중퇴하고 온라인에서 그들의 교육을 계속하거나 홈스쿨링을 받기로 결정할 수 있습니다. 다른 학교로 전학을 가는 것은 효과적이지 않을 수도 있습니다. 뉴욕시 학교의 연구 연맹 (Research Alliance)에 따르면 학습 환경은 학생의 성공에 중요한 역할을한다고 합니다.</td>
            </tr>
            <tr class = "second-dialog-lg">
              <td class = "uppertable" ><b>Ashley :</b></td>
              <td class = "lowertable" >학생들이 학교를 중퇴하는 것을 허용해서는 안 됩니다 우선, 학교를 중퇴한 9세에서 18세 사이의 학생들은 서울에서 매달 20만 원의 보조금을 받습니다. 이 정책의 목표는 학생들이 책을 사고 온라인 강좌를 수강하도록 장려하는 것이지만, 이 돈은 다른 용도로 사용될 수도 있습니다 어쩌면 이 돈을 비디오 게임이나 과자, 옷이나 불법적인 것을 사기 위해 사용할지도 모릅니다 이런 점을 감안한다면, 이런 보조금은 완전히 세금 낭비입니다.</td>
            </tr>
  
            </table>
  
  
        </div>
  
      <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Questions</h3>
  
        <div style="padding : 16px;">
  
          <ol style="margin: 12px;">
            <li>How important is education to you?</li>
            <li>In what ways does dropping out of school affect a student’s life?</li>
            <li>What causes students to drop out of school?</li>
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
  