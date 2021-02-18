<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/piano-guitar-wooden-background-closeup_169016-1999.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Pianos Versus Guitars
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
      <td class = "lowertable" >There is a myriad of reasons why the piano is better than the guitar. First and foremost, it is easier to learn how to play the piano. According to elitemusic.ca, “For a beginner, it is easier to learn and memorize the notes on a piano because they repeat in the same pattern across all the keys.” The site added, “On guitar, the note patterns are a little more complex because each string has a different arrangement of notes.” Guitars are known to scare away beginners. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >The piano has a very classical sound that may come across as too outdated or serious. The guitar is more versatile, as it can sound very romantic, vibrant, or mysterious. It’s perfect for all types of genres, especially rock. According to takelessons.com, “Most rock enthusiasts prefer the guitar over the piano. Guitar is the quintessential rock instrument. Early rock and roll pioneers who played the guitar include Elvis Presley and Chuck Berry. They paved the way for later ‘rock guitar gods,’ from Jimi Hendrix to Jimmy Page.”</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>myriad</b> 무수함, 무수히 많음
        </p>
        <p>
          <b>outdated</b> 구식인
        </p>
        <p>
          <b>versatile</b> 다용도의, 다목적의
        </p>
        <p>
          <b>quintessential</b> 정수의, 전형의
        </p>
        <p>
          <b>pioneer</b> 개척자[선구자]
        </p>
         
         
         
         
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >피아노가 기타보다 나은 이유는 무수히 많습니다. 무엇보다도, 피아노 연주하는 법을 배우는 것이 더 쉽습니다. elitemusic.ca에 따르면 "초보자의 경우 피아노의 음표가 모든 건반에서 동일한 패턴으로 반복되기 때문에 배우고 암기하는 것이 더 쉽습니다." "기타에서는 각 줄이 음표 배열이 다르기 때문에 음표 패턴이 조금 더 복잡합니다."라고 덧붙였습니다. 기타는 초보자를 겁주어 쫓는 경향이 있는 악기로 알려져 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >피아노는 너무 구식이거나 근엄할 수도 있는 매우 고전적인 소리를 가지고 있습니다. 기타는 매우 낭만적이거나 생생하고 신비하게 들릴 수 있기 때문에 더 다양합니다. 모든 유형의 장르, 특히 록(rock)에 적합합니다. takelessons.com에 따르면“대부분의 록 애호가들은 피아노보다 기타를 선호합니다. 기타는 전형적인 록 악기입니다. 기타를 연주 한 초기 로큰롤(rock and roll) 개척자에는 엘비스 프레슬리(Elvis Presley)와 척 베리(Chuck Berry)가 있습니다. 그들은 나중에 지미 헨드릭스(Jimi Hendrix)에서 지미 페이지(Jimmy Page)에 이르기까지 훗날의 '록 기타 신들'을 위한 길을 열었습니다.”</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you know how to play any musical instrument? Which ones can you play or would like to learn?</li>
          <li>If you can choose to play between a piano and a guitar, which one will you choose and why?</li>
          <li>Which do you think is easier to learn, guitar or piano?</li>
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
