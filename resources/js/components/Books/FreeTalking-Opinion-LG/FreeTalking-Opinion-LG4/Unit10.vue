<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/chef-with-his-arms-crossed-white-background_1368-11925.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Universal Basic Income A Good Idea?
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
      <td class = "lowertable" >Many people around the world suffer from poverty, and universal basic income can reduce it. The African country of Namibia tested a UBI program from 2007- 2017. During that period, poverty rates went from 76 percent to 37 percent. Child malnutrition also fell from 42 percent to 17 percent. In addition, Alaska used to rank at No. 30 out of 50 in terms of income inequality in the United States. However, thanks to its UBI program, which was implemented in 1976, Alaska now ranks at No. 2.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >People should have jobs to make money. Otherwise, they might lose their drive to work. Charles Wyplosz, a professor at the Graduate Institute in Geneva, says, “If we pay people unconditionally to do nothing, they will do nothing.” He also explained that this will lead to a less effective economy. Economist Allison Schrager says a strong economy requires people who are motivated to work hard. According to bostonfed.org, Americans worked less in the 1970s and ’60s, when a pilot UBI program was in effect. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>periodic</b> 주기적인
        </p>
        <p>
          <b>pilot</b> 시험적인
        </p>
        <p>
          <b>poverty</b> 가난, 빈곤
        </p>
        <p>
          <b>malnutrition</b> 영양실조(증)
        </p>
        <p>
          <b>drive</b> 투지, 추진력
        </p>
        <p>
          <b>unconditionally</b> 무조건으로
        </p>
       
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >전 세계 많은 사람들이 빈곤으로 고통 받고 있으며 보편적 인 기본 소득으로 인해 빈곤층이 줄어들 수 있습니다. 아프리카 국가 나미비아는 2007-2017년 UBI 프로그램을 테스트했습니다. 그 기간 동안 빈곤율은 76 %에서 37 %로 증가했습니다. 아동 영양 실조도 42 %에서 17 %로 떨어졌습니다. 또한 알래스카는 미국의 소득 불평등 측면에서 50 위 중 30 위를 차지했습니다. 그러나 알래스카는 1976 년에 시행 된 UBI 프로그램 덕분에 현재 2 위에 올라있습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >사람들은 돈을 벌기 위한 직업을 가져야 합니다. 그렇지 않으면 일을 하기 위한 투지를 잃을 수도 있습니다. 제네바(Geneva,) 대학원의 찰스 와이플로스 (Charles Wyplosz )교수는 "우리가 사람들에게 무조건적으로 아무 것도 하지 않으면 그들은 아무 것도 하지 않을 것입니다."라고 말합니다. 그는 또한 이것이 덜 효과적인 경제로 이어질 것이라고 설명합니다. 경제학자 앨리슨 슈라거(Allison Schrager )는 경제가 튼튼하기 위해서는 열심히 일할 의욕을 가진 사람들이 필요하다고 말합니다. 보스턴피드 닷 오알지(bostonfed.org)에 따르면, 미국인은 1970 년대와 60 년대에 시험적 UBI 프로그램이 시행되었을 때 보 다 덜 효과적이었습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are your thoughts on the Universal Basic Income Program?</li>
          <li>Do you believe that the Universal Basic Income program could help reduce poverty? Why or why not?</li>
          <li>Would the implementation of the said program influence a person’s motivation to work? How?</li>
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
