
<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/free-climber-young-man-climbing-artificial-boulder-indoors_155003-7643.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should kids be allowed to do extreme sports?
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
      <td class = "lowertable" >Everyone knows that exercise is good for you. The problem is that traditional sports are no longer attractive to our generation. But the thrill of these exciting sports just might do the trick to get kids to work out! If extreme sports can get children out of the house instead of staying home for video games, it will be a good thing. Not to mention, extreme sports can also teach young people how to take more risks in their lives.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Have you ever flown through the air for several meters before landing? Extreme sports may look cool, but they’re just too dangerous for children. Compared to soccer, basketball, or baseball, the risk is too high! Thrilling sports can seriously hurt players and may even lead to their deaths. Being healthy is important, but what is the point of becoming fit if you die during the exercise? The damage caused by these dangerous sports isn’t just limited to broken legs or arms, but can have much more serious consequences.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>traditional</b>  전통[인습]적인, 전통을 따르는
        </p>
        <p>
          <b>extreme</b> 극도의, 극심한
        </p>
        <p>
          <b>risk</b> 위험
        </p>
        <p>
          <b>dangerous</b> 위험한
        </p>
        <p>
          <b>consequence</b> 결과
        </p>
        
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >모두가 운동이 좋은 것을 알고 있습니다. 문제는 우리 세대에게 전통적인 운동이 더 이상 매력적이지 못한 것입니다. 하지만 이러한 재미있는 운동의 스릴감이 어린이들이 운동하게 할 겁니다! 극한 스포츠가 아이들이 집에서 비디오 게임을 하며 집에만 있지 않고 나가게 한다면, 좋은 것일 겁니다. 거기다가 극한 스포츠가 젊은이들에게 더욱 모험을 할 수 있도록 가르쳐 줄 수 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >착지하기 전에 몇 미터씩 공기 속을 날아 본 적이 있습니까? 극한 스포츠는 멋있어 보이지만, 어린이들에게는 너무 위험합니다. 축구, 농구, 야구에 비하면 위험이 너무 높아요! 흥분되는 운동은 심각하게 선수를 다치게 할 수 있으며, 죽게 할 수도 있습니다. 건강해지는 것도 중요합니다, 하지만 운동하다가 죽으면 건강이 무슨 소용일까요? 이러한 위험한 운동으로 일어나는 부상은 부러진 다리나 팔에 그치지 않지만, 하지만 더욱 심각한 결과를 만들어 낼 수 있습니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What comes to your mind when you hear the term “extreme sports”?</li>
          <li>Have you tried or thought of trying any extreme sport? If yes, what kind and why??</li>
          <li>Do you think kids should be allowed to do these kinds of activities?</li>
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
