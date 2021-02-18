<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/friends-social-media_53876-90180.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Do Smartphones Make People Less Sociable?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class="line-top-opinion1">
  </div>

  <h3  class = "lower-header-opinion1 white--text" >Topic</h3>
  <div style = "line-height: 1.6;">
    <div style="padding : 16px;">   

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>A :</b></td>
      <td class = "lowertable" >With smartphones, you can shop online and even do online banking.
      You can see how your friends are doing through social media, too.
      Naturally, we get fewer chances to step outside and physically meet people.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>B :</b></td>
      <td class = "lowertable" >Smartphones are helpful in finding good tourist spots and restaurants.
      They also help you to contact people easily.
      So what matters is not the smartphone, but one's personality.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>sociable</b> 사람들과 어울리기 좋아하는
        </p>
        <p>
          <b>naturally</b> 자연스럽게
        </p>
        <p>
          <b>few</b> 적은
        </p>
        <p>
          <b>physically</b> 실제로
        </p>
        <p>
          <b>tourist spot</b> 관광명소
        </p>
        <p>
          <b>contact</b> 연락하다
        </p>
        <p>
          <b>matter</b> 중요하다
        </p>
        <p>
          <b>personality</b> 성격..
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

                      <p class = "korean">
                        <b>
                        스마트폰은 사람들이 다른 사람들과 덜 어울리게 하나요?
                        </b>
                      </p>

                      <table class = "standard-table">

                       <tr>
                        <td class = "uppertable" ><b>A :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >스마트폰으로, 여러분은 온라인 쇼핑을 할 수 있고 심지어 온라인 뱅킹도 할 수 있습니다.
                          여러분은 또 소설 미디어를 통해 친구들이 어떻게 지내고 있는지 볼 수도 있습니다.
                          자연스럽게 우리는 밖에 나가서 사람들을 신체적으로 만날 확률이 줄어 듭니다.</td>
                      </tr>
                      <tr style="color:#1565C0;">
                        <td class = "uppertable" ><b>B :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >스마트폰은 좋은 관광지와 레스토랑을 찾는 데 도움이 됩니다.
                          또한 사람들에게 쉽게 연락 할 수 있도록 도와줍니다.
                          중요한 것은 스마트 폰이 아니라 개인의 성격입니다.</td>
                      </tr>

                    
                      </table>

       
      </div>
     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are the advantages and disadvantages of using smartphones?</li>
          <li>How often do you use your smartphone and check your social media accounts in a day?</li>
          <li>How have smartphones produced anxiety in any of your social settings in real life?</li>
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
