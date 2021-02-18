<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/teen-girl-with-lot-books_155003-4094.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Homework Beneficial?
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
      <td class = "lowertable" >Many studies show that homework improves a student’s grades, test results, and their likelihood of attending university. A research paper in the High School Journal states that spending at least an hour doing homework results in significantly better test scores. Studious children tend to score about 40 points higher on the math portion of the SAT than those who spend little time on homework. Furthermore, the Institute for the Study of Labor discovered that the amount of homework affects a student’s grade point average.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >According to a poll of Californian high school students, around 59 percent said that they had too much homework. An overwhelming 82 percent said they were often stressed by homework, and about 43 percent stated that homework was their biggest source of stress. Moreover, the American Educational Research Association once said, “Whenever homework crowds out social experience, outdoor recreation, and creative activities, and whenever it usurps time that should be devoted to sleep, it is not meeting the basic needs of children and adolescents.” </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>likelihood</b> 가능성
        </p>
        <p>
          <b>paper</b> 논문
        </p>
        <p>
          <b>significantly</b> 상당히
        </p>
        <p>
          <b>studious</b> 학구적인
        </p>
        <p>
          <b>affect</b> 영향을 미치다
        </p>
        <p>
          <b>grade point average</b> 평균 평점
        </p>
        <p>
          <b>poll</b> 여론 조사
        </p>
        <p>
          <b>overwhelming</b> 압도적인
        </p>
        <p>
          <b>crowd out</b> 밀어내다
        </p>
        <p>
          <b>outdoor</b> 야외의
        </p>
        <p>
          <b>recreation</b> 레크리에이션
        </p>
        <p>
          <b>usurp</b> 빼앗다
        </p>
        <p>
          <b>adolescent</b> 청소년
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >많은 연구들이 숙제가 학생의 성적, 시험 결과, 그리고 그들의 대학에 다닐 가능성을 높인다는 것을 보여줍니다. 고등학교 저널의 한 연구 논문은 숙제를 적어도 한 시간 하면 테스트 성적이 현저히 향상된다는 결과를 말합니다. 학업 성취도가 높은 아이들은 숙제에 시간을 거의 소비하지 않는 학생보다 SAT의 수학 부분에서 약 40점 높은 점수를 얻는 경향이 있습니다. 또한 노동 연구원은 숙제의 양이 학생의 학점 평균에 영향을 미친다는 사실을 발견했습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >캘리포니아 고등학생들의 여론 조사에 따르면 약 59 %가 숙제가 너무 많다고 답했습니다. 압도적 인 82%가 종종 숙제로 인해 스트레스를 받았다고 답했으며, 43%는 숙제가 스트레스의 가장 큰 원인이라고 말했습니다. 또한 미국 교육 연구 협회 (American Educational Research Association)는 "숙제가 사회적 경험, 야외 레크리에이션, 창의적인 활동을 몰아낼 때마다, 잠자는데 써야 할 시간을 낭비할 때마다 어린이와 청소년의 기본적인 욕구를 충족시키지 못한다"고 말했습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>How would you describe yourself as a student?</li>
          <li>Why is homework given? How does it help a student?</li>
          <li>In what ways can homework be stressful?</li>
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
