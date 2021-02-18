<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/red-chilli-paste-black_1150-25548.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Spicy Food Healthy?
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
      <td class = "lowertable" >Spicy food is good for you. According to a recent study in the British Medical Journal, “Compared with those who ate spicy foods less than once a week, those who consumed spicy foods six or seven days a week showed a 14 percent relative risk reduction in total mortality.” In simpler terms, this means that spicy foods could help you live longer. In addition, they may help with weight loss. According to an analysis of 90 different studies, spicy foods reduce appetite and increase energy. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Eating spicy food can have detrimental effects. First of all, spicy foods can trigger abdominal pain. According to a study done by Korean and Japanese researchers in 2016, spicy foods can cause gastrointestinal symptoms in people with indigestion and irritable bowel syndrome. Moreover, capsaicin can thin blood. This can be a huge problem for people who are taking certain medications. Finally, spicy foods can be especially painful for people with hemorrhoids. Eating spicy food can dramatically slow down the time it takes to heal. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>discomfort</b> (신체적인) 불편
        </p>
        <p>
          <b>bear</b> 참다, 견디다
        </p>
        <p>
          <b>mortality</b> 사망(률)
        </p>
        <p>
          <b>appetite</b> 식욕
        </p>
        <p>
          <b>detrimental</b> 해로운
        </p>
        <p>
          <b>trigger</b> 촉발시키다
        </p>
        <p>
          <b>gastrointestinal</b> 위장의
        </p>
        <p>
          <b>hemorrhoid</b>  치질
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >매운 음식이 몸에 좋습니다. 영국 의학 저널의 최근 연구에 따르면, "주 1회 이하의 매운 음식을 먹은 사람들과 비교했을 때, 일주일에 6, 7일 동안 매운 음식을 먹은 사람들은 총 사망률에서 14%의 상대적인 위험 감소를 보였습니다." 간단히 말해서, 이것은 매운 음식이 여러분이 더 오래 살 수 있도록 도와줄 수 있다는 것을 의미합니다. 게다가, 체중 감량에 도움을 줄 수 있습니다. 90가지 다른 연구 결과를 분석한 결과, 매운 음식은 식욕을 줄이고 에너지를 증가시킨다고 합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >매운 음식을 먹는 것은 해로운 영향을 미칠 수 있습니다. 우선 매운 음식은 복통을 유발할 수 있습니다. 2016년 한국과 일본 연구진이 실시한 연구에 따르면 매운 음식은 소화불량과 자극성 장 증후군을 가진 사람들에게 위장 증상을 일으킬 수 있다고 합니다. 게다가 캡사이신은 혈액을 묽게 할 수 있습니다. 이것은 특정한 약을 복용하는 사람들에게 큰 문제가 될 수 있습니다. 마지막으로, 매운 음식은 치질이 있는 사람들에게 특히 고통스러울 수 있습니다. 매운 음식을 먹는 것은 치유하는데 걸리는 시간을 극적으로 늦출 수 있습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Why do some people prefer their food spicy and others don’t?</li>
          <li>In your opinion, what is spicy food best paired with?</li>
          <li>Does spicy food lead to more diseases rather than it is beneficial to a person's health? How?</li>
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
