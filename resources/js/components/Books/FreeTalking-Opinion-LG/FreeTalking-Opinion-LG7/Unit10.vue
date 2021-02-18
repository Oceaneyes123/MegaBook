<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/group-diverse-friends-holding-movie-emoticons_53876-71065.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Comedy Movies Versus Horror Movies

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
      <td class = "lowertable" >Comedy movies are healthy because they make us laugh. Laughter has a multitude of benefits, including an improved immune system. According to mayoclinic.org, positive thoughts involving laughter release neuropeptides, which help fight stress and a variety of illnesses. Laughing soothes tension, too. Moreover, Time magazine says that laughter can even relieve pain. Surprisingly, laughing causes the body to make its own natural pain relievers. It also enhances the endorphins released by your brain, triggering positive feelings. No wonder laughter is the best medicine!</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >We should all watch more horror movies. They can help people with anxiety and fear. Studies show that anxiety from movies has positive connections to several parts of the brain. According to Mathias Clasen, who studies the effects of watching horror and thriller films, “Exposure to horror films can be gratifying when the negative emotions caused by the film are manageable. Moreover, there’s psychological distance when we watch a horror film. We know it’s not real. At least, some parts of our brain know it isn’t real.”</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>multitude</b> 아주 많은 수, 다수
        </p>
        <p>
          <b>soothe</b> (통증 등을) 누그러뜨리다[완화시키다]
        </p>
        <p>
          <b>tension</b> 긴장[불안]
        </p>
        <p>
          <b>trigger</b> 촉발시키다
        </p>
        <p>
          <b>anxiety</b> 불안(감)
        </p>
        <p>
          <b>gratifying</b> 흐뭇한, 기쁜
        </p>
        <p>
          <b>manageable</b> 관리[감당처리]할 수 있는
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >코미디 영화는 우리를 웃게 만들기 때문에 건강합니다. 웃음은 면역체계를 향상시키는 것을 포함하여 많은 이점을 가지고 있다. mayoclinic.org에 따르면 웃음과 관련된 긍정적인 생각은 스트레스와 다양한 질병과 싸우는 데 도움이 되는 신경 펩티드를 분비합니다. 웃음은 긴장도 누그러뜨립니다. 게다가, 타임지는 웃음이 심지어 고통을 덜어줄 수 있다고 말합니다. 놀랍게도 웃음은 신체가 자연적인 진통제를 만들게 합니다. 또한 뇌에서 방출되는 엔돌핀을 강화하여 긍정적인 감정을 유발합니다. 웃음이 최고의 약이라는 것은 당연합니다!</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >우리 모두 공포 영화를 더 많이 봐야 합니다. 그것들은 불안과 두려움을 가진 사람들을 도울 수 있습니다. 영화에서 나오는 불안감이 뇌의 여러 부분과 긍정적인 연관성이 있다는 연구결과가 나왔습니다. 공포와 스릴러 영화를 보는 효과를 연구하는 Mathias Clasen에 따르면 “영화로 인한 부정적인 감정을 감당할 수 있을 때 공포 영화에 대한 노출은 만족스러울 수 있습니다. 더구나 공포영화를 볼 때는 심리적 거리감이 있습니다. 우리는 그것이 진짜가 아니라는 것을 압니다. 적어도 우리 뇌의 일부는 그것이 진짜가 아니라는 것을 알고 있습니다.” </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like watching movies? What is your favorite movie?</li>
          <li>If you were to choose between watching horror or comedy movies, what will you choose?</li>
          <li>What do you think is the best movie genre?</li>
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
