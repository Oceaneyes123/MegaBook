<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/china-calligraphy-ink-paintbrush-handwriting-white_1417-483.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Learn Chinese?
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
      <td class = "lowertable" >Knowing Chinese comes with many advantages. Chinese has many dialects, but the most commonly spoken dialect is Mandarin. It is spoken by nearly 900 million people. Mandarin is spoken in many countries around the world, including Malaysia, Taiwan, Singapore, Indonesia, Thailand, Brunei, the Philippines, and Mongolia. So if you want to travel to another country, knowing Chinese will be very helpful. Also, if you need to do business in China or a Chinese-speaking country, you can converse in Chinese without an interpreter’s help.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Complexity is one of the main reasons why we should not learn Chinese. According to the U.S. Foreign Service Institute, Chinese is a Category IV Language, which means it takes at least 88 weeks of Chinese classes to speak the language somewhat fluently. The Chinese language does not use an alphabet. Instead, you use symbols that contain numerous strokes. In addition, most Chinese dialects are tonal. Korean and English are not tonal. Tones affect the meaning of a sound, so it’s important to master them.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>rich</b> 다채로운, 풍요로운
        </p>
        <p>
          <b>dialect</b> 방언
        </p>
        <p>
          <b>converse</b> 대화를 나누다
        </p>
        <p>
          <b>interpreter</b> 통역사
        </p>
        <p>
          <b>complexity</b> 복잡함
        </p>
        <p>
          <b>somewhat</b> 어느 정도
        </p>
        <p>
          <b>fluently</b> 유창하게
        </p>
        <p>
          <b>stroke</b> (글씨의) 획
        </p>
        <p>
          <b>tonal</b> 성조의
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >중국어를 아는 것은 많은 장점을 가지고 있습니다. 중국어에는 많은 방언이 있지만 가장 일반적으로 사용되는 방언은 만다린(Mandarin )입니다. 거의 9억 명의 사람들이 사용합니다. 만다린은 말레이시아(Malaysia), 대만, 싱가포르(Singapore), 인도네시아(Indonesia), 태국, 브루나이(Brunei), 필리핀(Philippines), 몽골 등 세계 여러 나라에서 사용됩니다. 그래서 여러분이 다른 나라로 여행하고 싶다면, 중국어를 아는 것이 매우 도움이 될 것입니다. 또한 중국이나 중국어권 국가에서 사업을 해야 하는 경우 통역사의 도움 없이 중국어로 대화 할 수 있습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >복잡성은 우리가 중국어를 배워서는 안 되는 주된 이유 중 하나입니다. 미국 외무 연구소 (US Foreign Service Institute)에 따르면 중국어는 카테고리4(Category IV )언어로서 언어를 유창하게 구사하는 데 적어도 88 주의 중국어 수업이 필요하다는 것을 의미합니다. 중국어는 알파벳을 사용하지 않습니다. 대신, 많은 획을 포함하는 기호를 사용합니다 또한, 대부분의 중국 방언은 성조입니다 한국어와 영어는 성조가 아닙니다. 음은 소리의 의미에 영향을 미치므로, 음을 숙달하는 것이 중요합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What do you think about the Chinese language?</li>
          <li>If given a chance, would you try to study and learn Chinese?</li>
          <li>What other languages would you like to learn and be good at? Why?</li>
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
