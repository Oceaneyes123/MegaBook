<template>

    <div :style = "{fontSize: fontSize + 'px'}">
  
      <v-container fluid ma-0 pa-0>
  
        <v-layout column>
          <v-img src="https://image.freepik.com/free-photo/asian-elderly-couple-using-tablet-virtual-reality-simulator-playing-games-living-room_7861-1559.jpg" style="max-width: 100%; display:block; height: auto;">
  
          <v-layout
          align-end
          fill-height
          pa-0
          white--text
          >
  
          <transition name="slide-fade">
          <h1 v-if="showTitle" class = "upper-header-lg">Should Korean Get Rid Of Honorifics?
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
        <td class = "lowertable" >The Korean language’s honorific system makes it hard for people to grow close to one another, especially if there is a large age gap or difference in status. Westerners, especially Americans, are often described as carefree, open-minded people. This is partly due to English’s lack of honorifics. Unlike Korean, you are not required to call someone your senior, and you don’t need to use sentence structures that come across stiff and distant. Some might think this makes English a rude language, but its lack of honorifics makes it easier to build relationships.</td>
      </tr>
      <tr class = "second-dialog-lg">
        <td class = "uppertable" ><b>Victoria :</b></td>
        <td class = "lowertable" >The honorific system is one reason why foreigners find Korean so fascinating. For instance, there are different ways to say “eat,” and you’d use the polite form to tell your parents to eat something. There are many ways to make a sentence sound polite, and there are ways to make something sound casual or rude, too. The different speech levels and honorifics make Korean such a unique language. The more you learn Korean, the more interesting it gets. Compared to English, Korean is so much more expressive!</td>
      </tr>
  
      </table>
  
        <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Vocabulary</h3>
  
        <div style="padding : 16px;">
  
          <p>
            <b>extensive</b> 광범위한
          </p>
          <p>
            <b>honorific</b> 존댓말
          </p>
          <p>
            <b>complicated</b> 복잡한
          </p>
          <p>
            <b>tradition</b> 전통
          </p>
          <p>
            <b>westerner</b> 서양인
          </p>
          <p>
            <b>carefree</b> 속 편한
          </p>
          <p>
            <b>come across</b> 인상을 주다
          </p>
          <p>
            <b>stiff</b> 뻣뻣한
          </p>
          <p>
            <b>distant</b> 거리를 두는
          </p>
          <p>
            <b>fascinating</b> 대단히 흥미로운
          </p>
          <p>
            <b>expressive</b> 표현이 풍부한
          </p>
  
        </div>
  
        <div class ="line-lg">
        </div>
        <h3 class = "border-translate-lg white--text">해석</h3>
  
        <div style="padding : 16px;">
  
          <table class = "standard-table">
  
            <tr>
              <td class = "uppertable" ><b>David :</b></td>
              <td class = "lowertable" >한국어의 존칭어법 체계는 사람들이 사람들이 서로 가까워지기 어렵게 만듭니다. 특히 연령 차이나 지위의 차이가 큰 경우에 그렇습니다. 서양인들, 특히 미국인들은 종종 속편하고 개방적인 사람들이라고 묘사됩니다. 이것은 부분적으로 영어가 존칭어법이 부족하기 때문입니다. 한국어와 달리 당신은 누군가를 당신의 연장자라고 부를 필요가 없고, 뻣뻣하고 거리를 두는 인상을 주는 문장 구조를 사용할 필요가 없습니다. 누군가는 이것이 영어를 무례한 언어로 만든다고 생각할지 모르지만 영어의 존칭어법 부족은 관계를 형성하는 것을 더 쉽게 만듭니다. </td>
            </tr>
            <tr class = "second-dialog-lg">
              <td class = "uppertable" ><b>Victoria :</b></td>
              <td class = "lowertable" >존칭어법 체계는 외국인들이 한국어를 매우 흥미롭게 생각하는 하나의 이유입니다. 예를 들어 “먹다”를 말하는 다양한 방법이 있고, 당신은 부모님께 무언가를 드시라고 말하기 위해 공손한 형태를 사용할 것입니다. 문장이 공손하게 들리도록 만드는 많은 방법들이 있습니다. 그리고 어떤 것이 격식을 차리지 않거나 무례하게 들리도록 만드는 방법들도 있습니다. 서로 다른 말하기 레벨과 존칭어법이 한국어를 그토록 독특한 언어로 만듭니다. 당신이 한국어를 더 많이 배울수록 더 흥미로워 집니다. 영어와 비교하면 한국어는 훨씬 더 표현력이 있습니다! </td>
            </tr>
  
            </table>
  
  
        </div>
  
      <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Questions</h3>
  
        <div style="padding : 16px;">
  
          <ol style="margin: 12px;">
            <li>What can you say about the Korean language’s honorific system?</li>
            <li>Can people build relationships easily if there are no honorifics? Why or why not?</li>
            <li>Other than honorifics, how do you show respect and politeness?</li>
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
  