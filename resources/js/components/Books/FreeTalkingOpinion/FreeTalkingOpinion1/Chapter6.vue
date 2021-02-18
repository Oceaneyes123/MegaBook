<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/close-up-business-executives-gossiping-together_1170-2012.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should We Tell On Others?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div style="line-top-opinion1">
  </div>

  <h3  class = "lower-header-opinion1 white--text">Topic</h3>
  <div style = "line-height: 1.6;">
    <div style="padding : 16px;">   

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>A :</b></td>
      <td class = "lowertable" >I don't like a certain girl in our class.
      She always comes in late when there is a substitute.
      I think she is very disrespectful, and I want to tell the teacher when she comes back.
      You should always be on time for class!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>B :</b></td>
      <td class = "lowertable" >I think that we should just relax and let the substitute take care of it.
      By telling on another person, all we do is make ourselves look bad.
      She will get in trouble with her bad attitude.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>tell on</b> 고자질 하다
        </p>

        <p>
          <b>certain</b> 어떤
        </p>

        <p>
          <b>substitute</b> 대안, 대체
        </p>

        <p>
          <b>disrespectful</b> 무례한
        </p>

        <p>
          <b>get in trouble with</b> ~ ~로 곤란 에 빠지다
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

                      <p class = "korean">
                        <b>
                        해석 다른 사람에게 일러야 하나요?
                        </b>
                      </p>

                      <table class = "standard-table">

                       <tr>
                        <td class = "uppertable" ><b>A :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >나는 우리 반에서 어떤 여자애를 좋아하지 않아요.
                          그녀는 항상 어떤 일이 있을 때 늦게 와요. 나는 그녀가 매우 무례해서 그녀가 돌아왔을 때, 선생님께 말하고 싶어요.
                          여러분은 항상 수업에 제시간에 와야만 합니다!!</td>
                      </tr>
                      <tr style="color:#1565C0;">
                        <td class = "uppertable" ><b>B :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >나는 우리가 좀 느긋해져야 하고 다른 방법으로 그 일이 다뤄져야 한다고 생각해.
                          다른 사람에 대해 고자질 하는 것으로 우리가 하는 모든 일이 우리 자신을 좋지 않게 보이게 만들 뿐이야.
                          그녀는 그녀의 나쁜 행동으로 곤란에 빠질거야.</td>
                      </tr>

                    
                      </table>


                      <p class = "korean">
                        우리는 다른 사람을 일러야 할까요?
                      </p>

        


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Is it proper to tell on others regarding someone's bad attitude and behavior? Why?</li>
          <li>Do you usually overreact when you see someone displaying their bad behavior? Or, do you prefer ignoring it?</li>
          <li>Have you ever told someone regarding your friend's bad behavior? What was his/her reaction?</li>
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
