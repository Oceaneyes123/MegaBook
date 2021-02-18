<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/students-schooling-uniform-backpack-japanese_53876-30279.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Students Have To Wear School Uniforms?
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
      <td class = "lowertable" >Students who wear uniforms tend to focus on their education, not what they wear. According to the National Association of Secondary School Principals, “When all students wear the same outfit, they are less concerned about how they look and how they fit in with their peers. Thus, they can concentrate on their schoolwork.” Hillary Clinton once said, “Put the focus on school, not on what you’re wearing.” Chris Hammons, a school principal, stated that uniforms “provide for less distraction, less drama, and more of a focus on learning.”</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >School uniforms infringe upon students’ right to express their individuality. The U.S. Constitution states that everyone has the right to express themselves. According to the American Civil Liberties Union of Nevada, “Allowing students to choose their clothing is an empowering message from the schools that a student is a maturing person who is entitled to the most basic self-determination.” Social critic George Carlin once asked, “Don’t these schools do enough damage by making all these children think alike? Now they’re going to get them to look alike, too?” </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>peer</b> 또래, 동료
        </p>
        <p>
          <b>distraction</b> 집중을 방해하는 것
        </p>
        <p>
          <b>infringe</b> 침해하다
        </p>
        <p>
          <b>individuality</b> 개성
        </p>
        <p>
          <b>empower</b> 자율권을 주다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >교복을 입는 학생들은 그들이 입는 것이 아니라 그들의 교육에 집중하는 경향이 있습니다. 전국 중고등학교 교장협회 따르면, "모든 학생들이 같은 옷을 입을 때, 그들은 그들이 어떻게 보이고 또 그들의 또래들과 어떻게 어울리는지에 대해 덜 걱정한다. 따라서, 그들은 학업에 집중할 수 있다." 힐러리 클린턴 (Hillary Clinton)은 "여러분이 입고 있는 옷이 아니라 학교에 집중하라."예전에 말한적이 있습니다.. 크리스 해먼스(Chris Hammons) 교장은 교복이 "혼란을 줄이고, 극적인 상황이 적고, 공부에 더 집중할 수 있게 해준다"고 말했습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >교복은 학생들의 개성을 표현할 권리를 침해합니다. 미국 헌법에는 모든 사람이 스스로를 표현할 권리가 있다고 명시되어 있습니다. 네바다 주 미국 시민 자유 연맹 (Civil Liberties Union of Nevada)에 따르면 "학생들이 자신의 옷을 선택할 수 있도록 허용하는 것은 학생들이 가장 기본적인 자기 결정을 할 자격이 있는 성숙한 사람이라는 학교의 권위 있는 메시지입니다." 사회 평론가 조지 칼린 (George Carlin)은 "이 아이들이 모든 아이들을 똑같이 생각하게 만들면 이러한 학교는 충분한 피해를 주지 않을까요? 이제 그들은 그들도 똑같이 보이게 할 것입니다. "라고 이전에 물었습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Is it necessary for students to wear school uniforms? Why or why not?</li>
          <li>Do you think wearing uniforms lessens the pressure to fit in? Why or why not?</li>
          <li>In what other ways can students express their individuality?</li>
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
