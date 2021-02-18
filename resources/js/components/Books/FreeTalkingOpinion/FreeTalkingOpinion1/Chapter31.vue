<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/little-girl-holds-puppy-her-arms_8353-153.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is There Such a Thing as Being Too Nice?
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
      <td class = "lowertable" >If you are too nice to people, they will start Looking down on you! Do you want people to perceive you as pathetic? We live in a dog-eat-dog world. Be tough!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >There is a difference between being nice and being a pushover. Being sweet and caring are valuable traits. As long as you know how to be assertive, you can be as nice as you want.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>perceive</b> 여기다
        </p>
        <p>
          <b>pathetic</b> 한심한
        </p>
        <p>
          <b>dog-eat-dog</b> 남에게 지지 않으려는
        </p>
        <p>
          <b>tough</b> 강인한 
        </p>
        <p>
          <b>difference</b> 차이
        </p>
        <p>
          <b>pushover</b> 만만한 사람 
        </p>
        <p>
          <b>caring</b> 배려하는 
        </p>
        <p>
          <b>valuable</b> 소중한 
        </p>
        <p>
          <b>trait</b> 특성 
        </p>
        <p>
          <b>assertive</b> 자신의 생각을 분명히 말하는
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >만약 네가 사람들에게 너무 친절하다면, 그들은 너를 무시하기 시작할 거야! 사람들이 널 한심하다고 느끼길 바라니? 우리는 남에게 지지 않으려는 세상에 살고 있어. 강인해져!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">착하게 행동하는 것과 만만하게 행동하는 것에는 차이가 있어. 상냥하고 배려하는 것은 가치 있는 특성이야. 당당해지는 법을 아는 한, 얼마든지 착해 질 수 있어.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are the disadvantages of being nice?</li>
          <li>Have you ever experienced an inconvenience because of being too nice? What happened?</li>
          <li>Can you say ‘No’ to the people you care about? Why or why not?</li>
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
