<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/asian-man-barista-holding-tablet-checking-order-from-customer-coffee-cafe_1150-8047.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">High School Students Should Have Afterschool Jobs
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
      <td class = "lowertable" >Korean teens should try working part-time jobs. Many youths across the world have part-time jobs, whether at their parents’ stores, fastfood restaurants, or other businesses. Having a job has a number of benefits: earning pocket money, learning how to be on time and follow orders, realizing the value of work and money, opportunity to become friends with coworkers, and developing teamwork skills. These things cannot be learned in a classroom, so exposure to real life through a part-time job should be something all Korean youths should have the chance to experience.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Teens having part-time jobs are common worldwide, but this isn’t practical in Korea, mainly because of the Korean education system. Admission to college is the goal most students here are focused on, and having a job would distract from that urgent task. Their grades could also suffer. Because studying takes up so much of a Korean youth’s time, he or she should instead use spare time to spend with friends or family. Plus students could get the false impression that work is more important than school, especially after getting paid.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>pocket money</b> 용돈
        </p>
        <p>
          <b>real-world</b> 현실세계
        </p>
        <p>
          <b>coworker</b> 직장 동료
        </p>
        <p>
          <b>admission</b> 입학
        </p>
        <p>
          <b>spare</b> 여분의
        </p>
        <p>
          <b>suffer</b> 어떤 것에 나쁜 영향을 받아서 악화되다
        </p>
        <p>
          <b>false</b> 틀린 생각에 근거한
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >한국의 청소년들은 파트타임 근무를 해보아야 합니다. 전 세계 많은 청소년들은 부모님의 가게나, 패스트푸드 식당 그리고 다른 사업체 등에서 파트타임 근무를 합니다. 직업을 갖는 것은 수 많은 이점이 있는데, 이것에는 용돈 벌기, 시간을 어기지 않고 규칙을 따르는 법을 배우기, 일과 돈 그리고 동료들과 친구되는 기회의 가치를 깨닫기, 팀워크를 향상하기 등이 있습니다. 이러한 것들은 교실에서 배울 수 없는 것으로, 파트타임 근무를 통한 현실세계로의 노출이 모든 한국 청소년들이 가져야 할 경험해야 할 기회가 되어야 합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >청소년들이 파트타임 근무를 갖는 것은 세계적으로 흔한 일이지만, 한국에서는 주로 한국의 교육 시스템으로 인하여 실용적이지 못합니다. 대학 입학은 이곳의 대부분 학생들이 집중하는 목표이며, 직업을 갖는 것은 시급한 과제로부터 떨어지게 할 것입니다. 성적 또한 떨어질 것입니다. 공부가 한국 청소년들의 시간의 많은 부분을 소비하기에, 그 혹은 그녀는 대신 친구들이나 가족들과 시간을 보내기 위하여 여가 시간을 사용해야 합니다. 게다가 학생들은 급여를 받은 후에 일이 학교보다 중요하다는 거짓된 인상을 받을 수 있습니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Did you have an afterschool job when you were a student? Why or why not?</li>
          <li>How does an afterschool job affect a student’s performance?</li>
          <li>Do you think teens should have an afterschool job? Why or why not?</li>
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
