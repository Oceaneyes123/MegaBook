<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/paper-speech-bubbles-with-hello-different-languages_23-2148293456.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should a Single Universal Language Exist?
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
      <td class = "lowertable" >Having a single universal language makes sense in our modern world. We are all connected thanks to the internet. For globalization, a universal language is necessary.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Language is not only about communication. It is also about having a distinct identity. Different languages will remain as long as humans strive for individualism.</td>
    </tr>

    </table>

    </div>

      <div class = "standard-table">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>make sense</b> 말이 되다 
        </p>
        <p>
          <b>modern</b> 현대의 
        </p>
        <p>
          <b>connected</b> 연결된 
        </p>
        <p>
          <b>globalization</b> 세계화 
        </p>
        <p>
          <b>necessary</b> 필요한 
        </p>
        <p>
          <b>communication</b> 의사소통 
        </p>
        <p>
          <b>distinct</b> 확실한 
        </p>
        <p>
          <b>identity</b> 독자성 
        </p>
        <p>
          <b>remain</b> 남다 
        </p>
        <p>
          <b>strive</b> 분투하다 
        </p>
        <p>
          <b>individualism</b> 개성
        </p>

      </div>

      <div class = "standard-table">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >하나의 보편적인 언어를 갖는 것은 현대 세계에서 이치에 맞아. 우리는 모두 인터넷 덕분에 연결되어 있어. 세계화를 위해서는 보편적인 언어가 필요해</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >언어는 단지 의사소통에 관한 것만은 아니야 그것은 또한 뚜렷한 독자성을 갖는 것에 대한 것이지. 인간이 개성을 위해 노력하는 한 다른 언어들은 남아있을 거야.</td>
          </tr>
      
          </table>


      </div>

     <div class = "standard-table">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What other language would you like to be fluent in? Why?</li>
          <li>Do you think we should have only one language for everyone? Why or why not?</li>
          <li>Which language would you prefer to be the universal language? Why?</li>
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
