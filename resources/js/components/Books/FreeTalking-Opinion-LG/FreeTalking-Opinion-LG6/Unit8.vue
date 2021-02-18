<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/elevated-view-magnifying-glass-burnt-paper-knife-map_23-2147837103.jpgg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is History An Important Subject In School?
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
      <td class = "lowertable" >“Those who ignore the past are doomed to repeat it” is a very famous saying. History is the study of preceding events, and as we all know, human nature repeats itself. If we cannot learn history, we remain ignorant. If we forget about the bad things of the past like war, genocide, or slavery, we may repeat such horrors in newer and more horrible ways. History teaches us lessons and shows us the hindsight with which we can ensure such actions do not repeat themselves.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >History may be the study of the past, but we are currently in a present that requires more important knowledge. Science, economics, and languages: these are more important subjects right now than history. History is a hobby that masquerades as an important subject. What do we gain out of history that will help our globalized world? Why should we care about the name of Christopher Columbus’s ship when we should be learning Mandarin to better understand our Chinese neighbors. Globalization does not count on the past ? It counts on the present and the future.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>remain</b> ~ 상태로 남다
        </p>
        <p>
          <b>ignorant</b> 무지한
        </p>
        <p>
          <b>genocide</b> 집단 학살
        </p>
        <p>
          <b>slavery</b> 노예 제도
        </p>
        <p>
          <b>horror</b> 참상
        </p>
        <p>
          <b>hindsight</b> 뒤늦은 깨달음
        </p>
        <p>
          <b>masquerade</b> 가식, 가장
        </p> 
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >“과거를 무시하는 사람들은 그 과거를 되풀이하기 마련이다”라는 매우 유명한 말이 있습니다. 역사는 지나간 일들에 대한 공부이며, 우리가 다 알다시피 인간의 본성은 반복됩니다. 만약 우리가 역사를 배울 수 없다면, 우리는 무지하게 됩니다. 만약 전쟁, 집단 학살 그리고 노예제도와 같은 과거의 나쁜 일들에 대해 잊게 된다면, 우리는 더 새롭고 끔찍한 방식으로 그러한 참상들을 반복하게 될지도 모릅니다. 역사는 우리에게 교훈을 가르쳐주고, 그러한 행동들이 반복되지 않도록 보장해 주는 뒤늦은 깨달음을 줍니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >역사는 과거의 학문일 수 있지만, 우리는 더 중요한 지식을 요구하는 현재에 살고 있습니다. 과학, 경제학 그리고 언어학은 현재 역사보다 더 중요한 과목들입니다. 역사는 중요한 과목으로 가장한 취미입니다. 역사에서 우리가 세계화된 시대에서 도움이 될 것들을 얻을 수 있을까요? 우리가 중국의 이웃들을 더 잘 이해하기 위해 중국어를 배워야 할 때, 왜 크리스토퍼 콜럼버스의 배의 이름에 대한 신경을 써야 합니까? 세계화는 과거에 의존하지 않습니다 - 그것은 현재와 미래에 의존합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you think studying history is important? Why or why not?</li>
          <li>What are the advantages of studying history?</li>
          <li>What will happen if schools no longer teach history?</li>
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
