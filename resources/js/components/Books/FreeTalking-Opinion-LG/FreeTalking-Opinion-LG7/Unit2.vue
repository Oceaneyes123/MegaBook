<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/handsome-adult-man-perform-song-singing-into-microphone-standing-against-turquoise-wall_1258-23898.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Vocal Tone Versus Vocal Range
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
      <td class = "lowertable" >Vocal tone, which is also known as the timbre of one’s singing voice, is very important. It’s actually more important than range. Why? Well, we naturally prefer listening to people with attractive vocal tones. Likewise, we like it when someone has a nice, soothing speaking voice. Tone is also important because it lets you know who the singer is instantly. The Beatles, for example, aren’t exactly known for their vocal prowess. However, their voices are very unique, so the band is quite easy to recognize.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Tone is important, but it’s not as important as one’s vocal range. You can have the best tone in the universe, but if you have a small range, your music will be boring and lifeless. A song should have a wide range so that the listener can feel a variety of emotions. A song should take us on a journey, like a movie. According to songstuff.com, “It is important that listeners feel a sense of progress through a song. It’s all about movement within a piece.” </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">
        <p>
          <b>timbre</b> 음색
        </p>
        <p>
          <b>prowess</b> 뛰어난 기량
        </p>
        <p>
          <b>attractive</b> 매력적인
        </p>
        <p>
          <b>lifeless</b> 활기 없는
        </p>
        <p>
          <b>progress</b> ~으로 넘어가다
        </p>
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >노래하는 목소리의 음색이라고도 불리는 보컬 톤은 매우 중요합니다. 사실 음역대 보다 더 중요합니다. 왜요? 음, 우리는 자연스럽게 매력적인 음색을 가진 사람들을 듣는 것을 선호합니다 마찬가지로 우리는 누군가가 멋지고 마음이 편해지는 목소리를 가지고 있을 때 그것을 좋아합니다. 음색은 가수가 누구인지 즉시 알 수 있기 때문에 중요합니다. 예를 들어, 비틀즈는 그들의 뛰어난 기량 보컬로 정확히 알려져 있지 않습니다. 하지만, 그들의 목소리는 매우 독특해서, 그 밴드는 꽤 쉽게 알아볼 수 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >음색도 중요하지만, 음역대만큼 중요한 것은 아닙니다. 우주에서 최고의 음색을 낼 수 있지만, 음역대가 작다면 음악은 지루하고 활기가 없을 것입니다. 노래는 듣는 사람이 다양한 감정을 느낄 수 있도록 범위가 넓어야 합니다. 노래는 우리를 영화처럼 여행에 데려가야 합니다. songstuff.com에 따르면, "청중은 노래를 통해 진취감을 느끼는 것이 중요합니다. 한 곡 안에서 움직이는 것은 전부입니다."</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you listen to songs a lot? Who is your favorite singer?</li>
          <li>Does a singer need to have a unique voice tone?</li>
          <li>What do you think is more important? Voice tone or voice range?</li>
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
