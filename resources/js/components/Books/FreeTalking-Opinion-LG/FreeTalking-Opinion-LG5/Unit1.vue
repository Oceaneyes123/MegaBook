<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/student-studying-brainstorming-analying-campus-concept_53876-14034.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should University Education Be Free?
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
      <td class = "lowertable" >Many job applications require at least a bachelor’s degree, so it would be unfair not to make university education free for everyone. Tuition can be very expensive, so a lot of people with low incomes tend to skip college or apply for loans. As you may already know, loan debt is a huge problem. According to the American Federal Reserve System, the total college loan debt in the United States increases by billions every quarter. Furthermore, around 11 percent of student borrowers are more than 90 days delinquent.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Without tuition fees, universities would get funded by the government. Public schools rely on the government, and we all know that a lot of them aren’t exactly perfect. Many elementary, middle, and high schools use outdated textbooks, desks and chairs that are seconds away from completely collapsing, and - to be frank - some teachers just aren’t very good at teaching. Universities would drop in quality, and class sizes would be enormous. You get what you pay for. I mean, is quantity more important than quality?</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>student loan</b> 학자금 대출
        </p>
        <p>
          <b>colossal</b> 엄청난
        </p>
        <p>
          <b>crisis</b> 위기
        </p>
        <p>
          <b>collectively</b> 빚지고 있다
        </p>
        <p>
          <b>trillion</b> 1조
        </p>
        <p>
          <b>application</b> 지원서
        </p>
        <p>
          <b>delinquent</b> 채무를 이행하지 않는
        </p>
        <p>
          <b>outdated</b> 구식인
        </p>
        <p>
          <b>enormous</b> 막대한
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >많은 입사지원서는 최소한 학사 학위를 요구합니다. 그래서 모두에게 대학 교육을 무료로 해주지 않는 것은 불공평할 수 있습니다. 수업료는 매우 비쌀 수 있습니다. 그래서 저소득의 많은 사람들이 대학을 가지 않거나 대출을 신청하는 경향이 있습니다. 여러분이 이미 알겠지만 대출 부채는 큰 문제입니다. 미국 연방 준비 제도에 따르면 미국의 대학교 학자금 대출 부채 총액은 매 분기 수십억 달러 씩 증가합니다. 더욱이 11퍼센트 가량의 학생 대출자들은 90일 이상 연체자입니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >수업료 없이는 대학교가 정부에게 기금을 받을 수 없을 것입니다. 공립학교는 정부에게 의존하고 우리는 모두 그들 중 다수가 정확히 완벽하지 않다는 것을 알고 있습니다. 많은 초, 중, 고등학교는 구식 교과서, 완전히 부서지기 몇 초 전인 책상과 의자를 사용합니다. 솔직히 말하자면 일부 선생님은 교수법에 능숙하지 않습니다. 대학교는 질이 떨어질 것이고 교실 크기는 거대해질 것입니다. 제 말은, 양이 질보다 더 중요합니까? </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>How would you describe your life as a university student?</li>
          <li>Do you agree that university education should be free? Why or why not?</li>
          <li>What do you think would happen if university education becomes free?</li>
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
