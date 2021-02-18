<template>

    <div :style = "{fontSize: fontSize + 'px'}">
  
      <v-container fluid ma-0 pa-0>
  
        <v-layout column>
          <v-img src="https://image.freepik.com/free-photo/word-text-wooden-dices-brown-desk_23-2148101507.jpg" style="max-width: 100%; display:block; height: auto;">
  
          <v-layout
          align-end
          fill-height
          pa-0
          white--text
          >
  
          <transition name="slide-fade">
          <h1 v-if="showTitle" class = "upper-header-lg">Should we replace Konglish with new Korean words?
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
        <td class = "lowertable" >I’m proud to be a Korean who uses the Korean language! Why are we using a half version of English anyway? Learning English is important, but polluting our own language with Konglish words doesn’t seem to make sense. Korean is one of the best languages in the world! It’s scientifically and beautifully made, efficient and easy to learn, and is a testament to Korea’s culture. We can simply replace all our Konglish with actual Korean vocabulary. Plus, using Konglish only makes us look bad. </td>
      </tr>
      <tr class = "second-dialog-lg">
        <td class = "uppertable" ><b>Victoria :</b></td>
        <td class = "lowertable" >Konglish is great! It’s fun, easy, and has become a language of its own. It wasn’t always this way, but Konglish is now a part of Korea’s modern culture. Every Korean, whether young or old, uses Konglish on some level on a daily basis. From “cider” to “A/S,” Konglish has infused itself into people’s spoken and written language. With hundreds of variations already in use across the country, it is too late to replace them. Instead, they should be embraced as a part of Korea today! </td>
      </tr>
  
      </table>
  
        <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Vocabulary</h3>
  
        <div style="padding : 16px;">
  
          <p>
            <b>pollute</b> 오염시키다
          </p>
          <p>
            <b>efficient</b> 효율적인
          </p>
          <p>
            <b>testament</b> 증거
          </p>
          <p>
            <b>daily</b> 매일 일어나는, 나날의
          </p>
          <p>
            <b>basis</b> 근거, 이유
          </p>
          <p>
            <b>infuse</b> 불어넣다, 스미다, 주입하다
          </p>
          <p>
            <b>variation</b> 변화, 변형
          </p>
        </div>
  
        <div class ="line-lg">
        </div>
        <h3 class = "border-translate-lg white--text">해석</h3>
  
        <div style="padding : 16px;">
  
          <table class = "standard-table">
  
            <tr>
              <td class = "uppertable" ><b>David :</b></td>
              <td class = "lowertable" >의료 서비스는 가격이 감당할 수 있을 정도여야 하며 반드시 집행되어야 합니다. 우리가 사고와 사람들이 의료보험 없이 생각할 수 없을 정도의 빚을 지게 되는지 생각하면 이해가 됩니다. 코미디언 리자 다이는 지하철 플랫폼에서 졸도하였고 응급실에서 깨어났습니다. 건강보험 없이 그녀는 많은 비싼 수술과 치료를 지불해야 했습니다. 비록 긴급 의료지원이 있었지만, 그녀의 최종 청구서엔 405,000달러가 청구되었습니다. 우리가 사람들이 얼마나 많은 사고를 겪게 되는지 고려할 때 모두가 보호되어야 하는 것이 더 낫지 않을까요? </td>
            </tr>
            <tr class = "second-dialog-lg">
              <td class = "uppertable" ><b>Victoria :</b></td>
              <td class = "lowertable" >우리가 집행된 의료 서비스를 고려할 때 시스템은 사실 보이는 것보다 더 흠이 많습니다. 집행된 의료 서비스는 더 높은 세금을 의미하며 비록 사람들이 높게 세금을 부과받는다 하더라도 그것은 그들이 적절한 서비스를 받는다는 것을 의미하지 않습니다. 의료 서비스가 집행될 때 그것은 그들이 원하지 않는 것을 포함하는 시스템에 지불해야 한다는 것을 의미합니다. 여러분의 차가 가지지 않은 문제를 포함하는 자동차 보험 계획을 위해 지불하기를 강요받는 것이 옳을까요? 마찬가지로 여러분이 절대 사용하지 않을 무엇인가를 위해 지불하기를 강요받는 것이 옳을까요? </td>
            </tr>
  
            </table>
  
  
        </div>
  
      <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Questions</h3>
  
        <div style="padding : 16px;">
  
          <ol style="margin: 12px;">
            <li>How would you describe the healthcare system in your country?</li>
            <li>What do you think of universal healthcare?</li>
            <li>Do you believe that affordable healthcare should be enforced? Why or why not?</li>
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
  