<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/white-cyborg-finger-about-touch-human-finger-3d-rendering_117023-5.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Will Artificial Intelligence Technology Make Our Lives Better Or Worse??
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
      <td class = "uppertable" ><b>A :</b></td>
      <td class = "lowertable" >I believe that Al will change our lives for the better.
      For example, it can translate languages. In addition, Al robots can do jobs that are too dangerous for humans.
      We can send them to space missions.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>B :</b></td>
      <td class = "lowertable" >I think Al also has downsides to it. Al can learn on its own.
      It learns quickly and continuously.
      If it becomes too smart, many jobs might be replaced by AI robots.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>believe</b> 믿다
        </p>
        <p>
          <b>translate</b> 번역하다
        </p>
        <p>
          <b>language</b> 언어
        </p>
        <p>
          <b>dangerous</b> 위험한
        </p>
        <p>
          <b>send</b> 보내다
        </p>
        <p>
          <b>space</b> 우주
        </p>
        <p>
          <b>mission</b> 임무
        </p>
        <p>
          <b>downside</b> 불리한 면
        </p>
        <p>
          <b>continuously</b> 계속해서
        </p>
        <p>
          <b>replace</b> 대신하다
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

                      <p class = "korean">
                        <b>
                        인공 지능은 우리의 삶을 더 좋게 만들까, 더 나쁘게 만들까?
                        </b>
                      </p>

                      <table class = "standard-table">

                       <tr>
                        <td class = "uppertable" ><b>A :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >저는 AI(인공지능)가 우리의 삶을 더 좋게 변화시킬 것이라고 믿습니다.
                          예를 들어 언어를 번역 할 수 있습니다. 또한 AI 로봇은 인간에게 너무 위험한 작업을 수행 할 수 있습니다.
                          우리는 그들을 우주 임무에 보낼 수 있습니다.</td>
                      </tr>
                      <tr style="color:#1565C0;">
                        <td class = "uppertable" ><b>B :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >저는 AI는 또한 그것에 단점이 있다고 생각합니다.
                        AI 은 독자적으로 학습 할 수 있습니다.
                        그것은 빠르고 지속적으로 학습합니다 너무 똑똑해지면 많은 작업이 AI 로봇으로 대체 될 수 있습니다.</td>
                      </tr>

                    
                      </table>

    

      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What do you think about the emergence of artificial intelligence in the world?</li>
          <li>What are the benefits of using artificial intelligence?</li>
          <li>What are the changes that artificial intelligence will bring to the lives of the people?</li>
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
