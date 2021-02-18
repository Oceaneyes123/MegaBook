<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/prague-astronomical-clock_1401-363.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is Astrology Accurate?
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
      <td class = "lowertable" >My astrological sign is Scorpio. When I looked up the traits of a typical Scorpio, I was surprised! It felt like I was reading someone’s description of me. This kind of precision can’t be a coincidence!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Astrology suggests that there is a mystical relationship between astronomical wonders and the human world. Scientists reject astrology because it is not scientific.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>sign</b> 별자리 
        </p>
        <p>
          <b>Scorpio</b> 전갈자리 
        </p>
        <p>
          <b>trait</b> 특성
        </p>
        <p>
          <b>typical</b> 전형적인 
        </p>
        <p>
          <b>precision</b> 정확성 
        </p>
        <p>
          <b>coincidence</b> 우연의 일치 
        </p>
        <p>
          <b>suggest</b> 제안하다 
        </p>
        <p>
          <b>mystical</b> 신령스러운 
        </p>
        <p>
          <b>astronomical</b> 천문학의
        </p>
        <p>
          <b>wonder</b> 경이 
        </p>
        <p>
          <b>reject</b> 거부하다 
        </p>
        <p>
          <b>scientific</b> 과학적인
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >내 점성술 별자리는 전갈자리야 전형적인 전갈자리의 특징을 찾아봤을 때, 나는 깜짝 놀랐어! 마치 나에 대한 누군가의 설명을 읽고 있는 것 같았어. 이런 정확함은 우연이 될 수 없어!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">점성술은 천문학적인 경이로움과 인간 세계 사이에 신비로운 관계가 있다는 것을 암시해. 과학자들은 점성술이 과학적이지 않기 때문에 이를 거부해.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What is your astrological sign?</li>
          <li>What are the common characteristics of the people who belongs to the same astrological sign as you? Do you agree? Why or why not?</li>
          <li>Why do you think some people believe it and some people don’t?</li>
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
