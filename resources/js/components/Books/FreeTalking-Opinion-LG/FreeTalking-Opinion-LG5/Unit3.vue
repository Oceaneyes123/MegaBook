
<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/book-with-green-board-background_1150-3837.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should People Go To College?
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
      <td class = "lowertable" >College graduates make more money. According to upjohn.org, career earnings for college graduates are up to 136 percent higher than those of high school graduates. In the U.S., the average high school graduate’s income is said to be $35,615, while college graduates earn twice as much. Moreover, those with advanced degrees have an average income of $92,525. And if you want a good job, a college degree is necessary. Only 34 percent of jobs in the U.S. require a high school diploma or less.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >About 19 percent of students who enroll in college do not return for their sophomore year. On average, 41 percent of students who attend public colleges do not graduate within six years. As for private colleges, that number is higher: 77 percent. This results in a loss of money for these students, and they’re not the only ones who are wasting their cash. Every year, because of college dropouts, states lose $1.3 billion and the federal government loses $300 million due to wasted loans and scholarships. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>worth</b> ~의 가치가 있는
        </p>
        <p>
          <b>beneficial</b> 유익한
        </p>
        <p>
          <b>graduate</b> 졸업생
        </p>
        <p>
          <b>earning</b> 소득
        </p>
        <p>
          <b>advanced</b> 상급의
        </p>
        <p>
          <b>diploma</b> 졸업장
        </p>
        <p>
          <b>enroll</b> 등록하다
        </p>
        <p>
          <b>sophomore</b> 2 학년
        </p>
        <p>
          <b>dropout</b> 중퇴자
        </p>
        <p>
          <b>federal</b> 연방제의
        </p>
        <p>
          <b>loan</b> 융자금
        </p>
        <p>
          <b>scholarship</b> 장학금
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >대학 졸업자들이 더 많은 돈을 법니다. upjohn. org에 따르면 대학 졸업자의 직업 소득은 고등학교 졸업자의 직업 소득보다 최대 136% 높습니다. 미국에서는 평균적인 고등학교 졸업자의 소득은 3만5천6백1십5달러라고 합니다, 반면 대학 졸업자들은 두 배를 법니다. 더욱이 우수한 성적을 가진 이들은 평균 9만2천5백2십5달러의 소득이 법니다. 만약 당신이 좋은 직업을 갖고자 한다면 대학 학위는 필수입니다. 미국의 직업들 중 단지 34퍼센트만 고등학교 졸업장 또는 더 낮은 학벌을 요구합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >대학에 다니는 학생들 중 약 19 %는 2학년으로 돌아 가지 않습니다. 평균적으로 공립대학에 다니는 41퍼센트의 학생들은 6년 안에 졸업하지 않습니다. 사립 대학들의 경우 그 숫자는 77퍼센트로 더 높습니다. 이 결과는 학생들에게 돈의 손실을 가져오고, 돈을 낭비하고 있는 사람은 그들만이 아닙니다. 매년 대학 자퇴로 인해 주정부는 13억 달러를 잃고 연방 정부는 불필요한 융자와 장학금으로 3억 달러를 잃습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>How would you describe your college life?</li>
          <li>Do you believe that going to college is important? Why or why not?</li>
          <li>Do you think the opportunities for college graduates and high school graduates are the same? Why or why not?</li>
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
