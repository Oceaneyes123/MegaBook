<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/still-life-with-flower-vases-with-fruits-retro-radio_1150-19436.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Music And Art Classes Be Mandatory?
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
      <td class = "lowertable" >When I was in elementary school, I wasn’t a big fan of art or music. I could barely draw a circle, and my voice would always crack during music class. So I avoided taking any art or music classes in middle school. However, now that I’m going to high school soon, I regret my decision. Why? Well, I’ve been really interested in graphic design lately, and I love to sing now. When I go to high school, I’m going to take as many art and music classes as possible. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >In most elementary schools, students are required to take music and art. Those who show interest in these subjects can opt to take them in middle and high school. If you’re more cerebral or less artsy, you should have the choice to fill up your schedule with classes that actually intrigue you. According to the National Endowment for the Arts, 2.1 million Americans have a career in an art-related field. That may seem like a high number, but there are about 125.97 million people with full-time jobs in the United States.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>mandatory</b> 의무적인
        </p>
        <p>
          <b>curriculum</b> 교육과정
        </p>
        <p>
          <b>barely</b> 간신히
        </p>
        <p>
          <b>crack</b> (목소리가) 갈라지다
        </p>
        <p>
          <b>cerebral</b> 지적인
        </p>
        <p>
          <b>artsy</b> 예술적인
        </p>
        <p>
          <b>intrigue</b> 강한 흥미를 불러 일으키다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >제가 초등학교에 다닐 때 미술과 음악을 좋아하지 않았습니다. 저는 원도 간신히 그렸고, 제 목소리는 항상 음악 시간에 갈라지곤 했습니다. 그래서 중학교에서 미술과 음악 수업을 듣는 것을 피했습니다. 그러나 이제 곧 고등학교에 진학하기 때문에 저는 제 결정을 후회합니다. 왜냐구요? 글쎄요, 저는 최근 그래픽 디자인에 정말로 흥미를 느끼고 있고, 이제 노래하는 것을 아주 좋아합니다. 제가 고등학교에 가면 가능한 많은 미술과 음악 수업을 들을 예정입니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >대부분의 초등학교에서 학생들은 음악과 미술 수업을 들어야 합니다. 이 과목에 흥미를 보이는 학생들은 중학교와 고등학교에서 그 수업들을 듣도록 선택할 수 있습니다. 만약 당신이 더 이지적이거나 덜 예술적이라면 실제로 당신을 흥미롭게 하는 수업으로 당신의 일정을 채울 수 있는 선택권이 있어야 합니다. 국립 예술 기금에 따르면, 2백십만 명의 미국인이 예술 관련 분야에서 경력을 쌓았습니다. 그것은 높은 숫자처럼 보일지 모르지만 미국에는 1억2천5백9십7만 명의 풀타임 직업을 가진 사람들이 있습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What was your favorite subject? Why?</li>
          <li>Do you think it is important for all students to take music and arts class? Why or why not?</li>
          <li>Do music and arts classes help develop skills? If yes, what kind? If not, what do they do instead?</li>
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
