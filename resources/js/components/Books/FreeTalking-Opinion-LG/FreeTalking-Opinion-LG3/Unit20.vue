<template>

    <div :style = "{fontSize: fontSize + 'px'}">
  
      <v-container fluid ma-0 pa-0>
  
        <v-layout column>
          <v-img src="https://image.freepik.com/free-photo/flat-lay-arrangement-with-book-pencil-paper-airplane_23-2148389111.jpg" style="max-width: 100%; display:block; height: auto;">
  
          <v-layout
          align-end
          fill-height
          pa-0
          white--text
          >
  
          <transition name="slide-fade">
          <h1 v-if="showTitle" class = "upper-header-lg">Should You Study Abroad?
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
        <td class = "lowertable" >A lot of Korean students study in another country to improve their English skills. If you move to an English-speaking country, you’ll immerse yourself in the language. You’ll have daily conversations with native speakers, and doing so greatly improves your speaking skills. According to linguist Steve Kaufmann, it’s better to practice speaking a language face to face. Relying on books and memorization will only improve certain areas. Kaufmann recommends going “to the country where the language is spoken to get a lot of speaking experience.” </td>
      </tr>
      <tr class = "second-dialog-lg">
        <td class = "uppertable" ><b>Ashley :</b></td>
        <td class = "lowertable" >Why study abroad when you can learn English in Korea? There are thousands of English academies in Korea, so you can improve your English skills right here! Thanks to government regulations, private education costs have been going down. Studying abroad can get extremely expensive. According to the International Institute of Education, the average cost of studying in another country is around $18,000 per semester. This includes tuition, housing, and transportation costs, but the total may be higher depending on the country. It’s not worth it. </td>
      </tr>
  
      </table>
  
        <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Vocabulary</h3>
  
        <div style="padding : 16px;">
  
          <p>
            <b>immerse</b> ~에 몰두하다
          </p>
          <p>
            <b>linguist</b> 언어학자
          </p>
          <p>
            <b>rely</b> 의지하다
          </p>
          <p>
            <b>memorization</b> 기억, 암기
          </p>
          <p>
            <b>expensive</b> 비싼
          </p>
          <p>
            <b>semester</b> 학기
          </p>
          <p>
            <b>tuition</b> 수업(료)
          </p>
  
        </div>
  
        <div class ="line-lg">
        </div>
        <h3 class = "border-translate-lg white--text">해석</h3>
  
        <div style="padding : 16px;">
  
          <table class = "standard-table">
  
            <tr>
              <td class = "uppertable" ><b>Henry :</b></td>
              <td class = "lowertable" >많은 한국 학생들은 영어 실력을 향상시키기 위해 다른 나라에서 공부합니다. 영어권 국가로 넘어가면 그 언어에 몰입하게 됩니다. 여러분은 원어민들과 매일 대화를 할 것이고, 그렇게 하면 여러분의 말하기 능력이 크게 향상될 것입니다. 언어학자 스티브 카우프만(Steve Kaufmann)에 따르면, 언어를 직접 말하는 것을 연습하는 것이 더 좋다고 합니다. 책과 암기에 의지하는 것은 특정 분야만 개선될 것입니다. 카프만은 "많은 말하기 경험을 쌓기 위해 언어가 사용되는 나라로" 갈 것을 권장합니다. </td>
            </tr>
            <tr class = "second-dialog-lg">
              <td class = "uppertable" ><b>Ashley :</b></td>
              <td class = "lowertable" >한국에서 영어를 배울 수 있는데 왜 유학을 가나요? 한국에는 수천 개의 영어 학원이 있기 때문에, 여러분은 바로 이곳에서 영어 실력을 향상시킬 수 있습니다! 정부 규제 덕분에 사교육비가 계속 떨어지고 있습니다. 해외에서 공부하는 것은 매우 비쌀 수 있습니다. 국제교육원에 따르면, 다른 나라에서 공부하는 평균 비용은 한 학기에 약 18,000 달러입니다. 여기에는 등록금과 주거비, 교통비 등이 포함되지만, 국가에 따라 총액이 더 높을 수 있습니다. 그럴 가치도 없어요. </td>
            </tr>
  
            </table>
  
  
        </div>
  
      <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Questions</h3>
  
        <div style="padding : 16px;">
  
          <ol style="margin: 12px;">
            <li>Have you considered studying abroad? Why or why not?</li>
            <li>What are the benefits and downsides of studying abroad?</li>
            <li>How does studying abroad affect a person?</li>
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
  