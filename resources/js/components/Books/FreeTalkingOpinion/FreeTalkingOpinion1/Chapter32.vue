<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a6/Physiognomy.jpg/1280px-Physiognomy.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is Physiognomy Accurate?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class="line-top-opinion1">
  </div>

  <h3  class = "lower-header-opinion1 white--text">Topic</h3>
  <div style = "line-height: 1.6;">
    <div style="padding : 16px;">   

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>Jane :</b></td>
      <td class = "lowertable" >It’s a basic human instinct to judge others by their appearance. Why do you think our ancestors learned this behavior? It’s because a person’s true character always comes out through their physical form!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Deciding someone’s temperament and character from their appearance is ridiculous and shallow. Taking physiognomy seriously is dangerous because it lacks scientific evidence and commonly results in discrimination based on race and sex.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>basic</b> 기본적인 
        </p>
        <p>
          <b>instinct</b> 본능 
        </p>
        <p>
          <b>appearance</b> 외모 
        </p>
        <p>
          <b>behavior</b> 행동 
        </p>
        <p>
          <b>character</b> 성격 
        </p>
        <p>
          <b>physical</b> 신체적 
        </p>
        <p>
          <b>form</b> 모습 
        </p>
        <p>
          <b>temperament</b> 기질
        </p>
        <p>
          <b>shallow</b> 천박한 
        </p>
        <p>
          <b>evidence</b> 증거 
        </p>
        <p>
          <b>discrimination</b> 차별 
        <p>
          <b>race</b> 인종 
        </p>
        <p>
          <b>sex</b> 성별
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >외모로 남을 판단하는 건 인간의 기본 본능이야. 왜 우리 조상들이 이런 행동을 배웠다고 생각하니? 사람의 진정한 성격은 항상 신체적 형태로 나오기 때문이야!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">외모로 누군가의 기질과 성격을 결정하는 건 말도 안되고 천박해. 관상학을 심각하게 받아들이는 것은 과학적 증거가 부족하고 흔히 인종과 성에 따른 차별을 초래하기 때문에 위험해.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you believe that we can judge someone’s character by their appearance? Why or why not?</li>
          <li>According to the people you know, what is the usual first impression of you? Do you agree? Why or why not?</li>
          <li>What was your first impression of your best friend? Was your judgement right after getting to know them?</li>
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

p{

  margin-top: 10px;
}

h3{
  padding-top: 7px;

}


body{

  font-size: 16px;
}



</style>
