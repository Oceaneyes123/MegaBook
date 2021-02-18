<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/little-cute-girl-bed-with-toy_169016-2020.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Are Dreams Important in Our Daily Lives?
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
      <td class = "lowertable" >Some people think dreams are visions of the future or messages from otherworldly figures. I don’t believe in that hocus pocus! Dreams are random and serve no real purpose in the real world.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >According to scientists, studies suggest dreams help with memory processing, psychological and emotion balancing, and preparing for upcoming challenges. Dreams are important because they are another extension of our lives.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>vision</b> 환상 
        </p>
        <p>
          <b>otherworldly</b> 내세의 
        </p>
        <p>
          <b>hocus pocus</b> 터무니없는 말 
        </p>
        <p>
          <b>random</b> 무작위의
        </p>
        <p>
          <b>purpose</b> 목적 
        </p>
        <p>
          <b>memory</b> 기억력 
        </p>
        <p>
          <b>process</b> 처리하다 
        </p>
        <p>
          <b>psychological</b> 정신의 
        </p>
        <p>
          <b>balance</b> 균형을 잡다 
        </p>
        <p>
          <b>upcoming</b> 다가오는 
        </p>
        <p>
          <b>challenge</b> 도전 
        </p>
        <p>
          <b>extension</b> 연장
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >어떤 사람들은 꿈이 미래에 대한 비전이라고 생각하거나 다른 세상의 인물들로부터의 메시지라고 생각해. 난 그 터무니없는 말을 믿지 않아! 꿈은 무작위적이고 현실세계에서 진정한 목적에 도움이 되지 않아.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >과학자들에 따르면, 연구 결과가 꿈이 기억 처리, 심리적, 감정적 균형 조정, 그리고 다가오는 도전에 대비하는 데 도움이 된다는 것을 시사해. 꿈은 우리 삶의 또 다른 연장선이기 때문에 중요해.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you remember your dreams?</li>
          <li>Do you think your dreams have meaning?</li>
          <li>Based on the dialog, who do you agree with, Jane or Tom? Why?</li>
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
