<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/front-view-composition-with-different-books_23-2148851051.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Audiobooks Versus Paper Books
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
      <td class = "lowertable" >Listening to an audiobook is better than reading a regular book. According to Art Markman and Bob Duke, who are professors at the University of Texas, “Because you can’t go back and reread something, you’re much more likely to do a better job of trying to get the gist of what someone meant when you’re hearing them than when you’re reading.” To put it simply, audiobooks are like movies. In other words, you can enjoy the story better. With traditional books, your brain is busy looking at all the words.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >David Daniel, a professor of psychology at James Madison University, said that our minds occasionally wander when we read books and listen to audiobooks. According to Time magazine, “If you’re reading, it’s pretty easy to go back and find the point at which you zoned out. It’s not so easy if you’re listening to a recording.” In addition, Prof. Daniel conducted a study and found that students who listened to a podcast lesson performed worse on a quiz than those who read the same lesson on paper.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>gist</b> (말·글·대화의) 요지[골자]
        </p>
        <p>
          <b>occasionally<b> 가끔
        </p>
        <p>
          <b>wander</b> 다른 데로 팔리다[흐르다]
        </p>
        <p>
          <b>zone out</b> 멍해지다
        </p>
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >오디오북을 듣는 것이 일반 책을 읽는 것보다 낫습니다. 텍사스 대학교의 교수인 아트 마크맨(Art Markman)과 밥 듀크(Bob Duke)에 따르면, "돌아가서 무언가를 다시 읽을 수 없기 때문에, 여러분이 그것들을 읽을 때 보다 들을 때 누군가가 무엇을 의미했는지에 대한 요지를 알아내려는 노력을 훨씬 더 잘 할 수 있습니다" 라고 합니다. 간단히 말해서 오디오 북은 영화와 같습니다. 다시 말해, 여러분은 이야기를 더 잘 즐길 수 있습니다. 전통적인 책을 보게 되면, 여러분의 뇌는 모든 단어를 보느라 바쁩니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >제임스 매디슨(James Madison) 대학의 심리학 교수인 데이비드 대니얼(David Daniel)은 우리가 책을 읽고 오디오북을 들을 때 때때로 우리의 마음이 딴청을 피운다고 말했습니다. 타임지에 따르면 “여러분이 읽는 중이라면, 뒤로 돌아가서 멍해진 지점을 찾는 것이 매우 쉽습니다. 녹음을 듣고 있으면 그렇게 쉬운 일이 아닙니다." 또한 다니엘 교수는 연구를 실시한 결과 팟 캐스트 강의를 듣는 학생들이 같은 강의를 종이로 읽은 학생들보다 퀴즈에서 더 나쁘다는 것을 발견했습니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like reading books? Why or why not?</li>
          <li>Have you ever tried listening to an audio book? If yes, how was it?</li>
          <li>If you were to choose between audio and paper books, what would you choose?</li>
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
