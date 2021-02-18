<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://singularityhub.com/wp-content/uploads/2018/11/young-gamer-playing-video-game_shutterstock_624801452-1068x601.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Mobile Games and Video Games
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
      <td class = "lowertable" >Computer and video games take too long to complete and require too much dedication. Mobile games are better because you can play them casually and conveniently stop whenever you want.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Mobile games usually use “freemium” methods to make money. That means they lure in people to play for free and then tempt them into buying extra features. Mobile gamers usually spend too much money for low-quality content.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>complete</b> 완료하다 
        </p>
        <p>
          <b>require</b> 필요하다 
        </p>
        <p>
          <b>dedication</b> 헌신 
        </p>
        <p>
          <b>casually</b> 무심히
        </p>
        <p>
          <b>conveniently</b> 편리하게 
        </p>
        <p>
          <b>method</b> 방법 
        </p>
        <p>
          <b>lure</b> 유인하다 
        </p>
        <p>
          <b>tempt</b> 유도하다 
        </p>
        <p>
          <b>extra</b> 추가의 
        </p>
        <p>
          <b>feature</b> 특징
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >컴퓨터와 비디오 게임은 완료하는 데 너무 오래 걸리고 헌신을 너무 많이 해야 해 모바일 게임은 무심하게 할 수 있고 원할 때 언제든지 편리하게 정지할 수 있기 때문에 더 좋아.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >모바일 게임은 보통 돈을 벌기 위해 "프리미엄" 방법을 써. 이것은 그들이 사람들을 무료로 게임을 유인한 다음 그들이 추가 기능을 구매하도록 유혹한다는 것을 의미 해 모바일 게이머들은 보통 저품질 컨텐츠에 너무 많은 돈을 소비해.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like playing mobile games or video games? Why or why not?</li>
          <li>Which do you prefer, mobile or video games? Why?</li>
          <li>Have you ever spent money for a game? Why or why not?</li>
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
