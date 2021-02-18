<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/flat-lay-frame-with-orange-sticky-notes_23-2148389015.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Learning a Second Foreign Language Be Compulsory?
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
      <td class = "lowertable" >Yes, it should be mandatory to take a foreign language class other than English. English is not the only language that is spoken in the world. Yes, it’s often called the “international language” by many people, but you should learn another language as well. Let’s say a student wants to work in Japan when they become an adult. Learning Japanese would be extremely beneficial for them. According to author John Dougill, a professor at Ryukoku University, many Japanese people are not confident in their conversational skills.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Schools should not force students to take a second foreign language class. It could take an immense toll on their stress levels. Learning English is already hard enough, so to make a student learn another language on top of that would be daunting for them. There’s a phenomenon called second-language attrition, which is when you forget a foreign language. This happens if you don’t practice it enough or stop using it altogether, which is common after you graduate. You could’ve taken another class instead. </td>
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
          <b>confident</b> 자신감 있는
        </p>
        <p>
          <b>conversational</b> 대화의
        </p>
        <p>
          <b>take a toll</b> 큰 피해[타격]를 주다
        </p>
        <p>
          <b>daunting</b> 벅찬
        </p>
        <p>
          <b>attrition</b> 감소, 축소
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >예, 영어 이외의 외국어 수업을 수강해야 합니다. 세계에서 영어가 유일한 언어는 아닙니다. 그렇습니다. 많은 사람들이 종종 "국제 언어"라고 부르지만 다른 언어도 배워야 합니다 학생이 성인이 되어 일본에서 일하기를 원한다고 가정 해 봅시다 일본어를 배우는 것이 그들에게 매우 유익 할 것입니다. 류코쿠 대학 교수 인 존 두길에 따르면 많은 일본인들은 대화 기술에 자신이 없다고 합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >학교는 학생들에게 제2외국어 수업을 듣도록 강요해서는 안 됩니다. 그들의 스트레스 수준에 엄청난 타격을 줄 수 있습니다. 영어를 배우는 것은 이미 충분히 어렵기 때문에, 학생들이 그 위에 다른 언어를 배우게 하는 것은 그들에게는 벅찬 일일 것입니다. 외국어를 잊어 버렸을 때 발생하는 제 2 언어 소모 현상이 있습니다. 충분히 연습하지 않거나 아예 사용을 중단하면 이런 현상이 일어나는데, 졸업 후 흔히 볼 수 있습니다. 대신 다른 수업을 들을 수도 있었어요.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Why is language powerful?</li>
          <li>Based on your experience, in what instances was a foreign language useful?</li>
          <li>Would you want to learn a second foreign language? Why or why not?</li>
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
