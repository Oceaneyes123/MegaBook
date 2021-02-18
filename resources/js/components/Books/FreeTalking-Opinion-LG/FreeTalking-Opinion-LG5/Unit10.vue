<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/father-s-day-dad-son-reading-comic-book_23-2148511432.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Read Comic Books?
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
      <td class = "lowertable" >Comics are very helpful for young readers. Many difficult books have been simplified and complemented with pictures and comic-style dialogues to make it easier for children to learn. Many point to comics as a useful tool for children who want to learn how to read. The pictures and the content can keep them engaged and more excited about reading and learning. Comics are fun, and many modern educators believe in the power of fun education. Why should we make learning a struggle when we have interactive tools like comic books to help children get excited about reading?</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Comics may be helpful for children, but in many countries, they are often known to have negative effects. Many children often look at the pictures and ignore the dialogues. Instead, they look for hints and clues in the pictures to figure out what the story tells. In many cases, kids just look at the pictures and select their favorite illustrations, totally ignoring the story. If we look to comics as educational materials, we should also view things like movies and TV shows in the same way. Why should we give these things any power to teach children?</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>decades</b> 수십년
        </p>
        <p>
          <b>stepping stone</b> 디딤돌
        </p>
        <p>
          <b>detractor</b> 반대하는 사람
        </p>
        <p>
          <b>complement</b> 보충하다, 보완하다
        </p>
        <p>
          <b>dialogue</b> 대화하다
        </p>
        <p>
          <b>struggle</b> 애쓰다
        </p>
        <p>
          <b>interactive</b> 상호의
        </p>
        <p>
          <b>clue</b> 실마리
        </p>
       
 
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >만화는 어린 독자들에게 매우 도움이 된다. 아이들이 배우기에 더 쉽게 만들기 위해 많은 어려운 책들은 단순화되고 그림과 만화 형식의 대화들로 보충된다. 많은 사람들은 읽는 방법을 배우기를 원하는 아이들에게 만화를 유용한 도구로서 가리킨다. 그 그림들과 내용은 그들이 계속 관심을 갖고 있고 독서와 학습에 관하여 더 신나게 한다. 만화는 재미있고, 많은 현대 교육자들은 재미 있는 교육의 힘을 믿는다. 우리가 아이들이 독서에 대해 신나게 하는 만화 책과 같은 상호작용적인 도구를 가지고 있을 때 왜 우리는 학습을 힘든 일로 만들어야 하는가? </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >만화는 아이들에게 도움이 될지 모르지만, 많은 나라들에서, 만화는 가끔 부정적인 영향을 가진 것으로 알려져 있다. 많은 아이들은 가끔 그 그림들을 보고 그 대화들을 무시한다. 대신에, 그들은 그 이야기가 무엇을 말하는지를 이해하기 위해 그 그림 안에 있는 힌트와 단서를 찾는다. 많은 사례들에서, 아이들은 완전히 그 이야기를 무시하면서, 단지 그림을 보고 그들이 가장 좋아하는 그림을 선택한다. 만일 우리가 만화를 교육적인 자료로 생각해 본다면, 우리는 영화와 TV 프로그램과 같은 것들도 같은 방식으로 생각해야 한다. 왜 우리가 이런 것들에 아이들을 가르치기 위한 힘을 주어야 하는가? </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you read comic books? Can you name some of your favorites?</li>
          <li>What do you think of comics as a learning tool? Are they interactive or distracting? Why?</li>
          <li>Do you think comics would be an effective learning tool? Why or why not?</li>
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
