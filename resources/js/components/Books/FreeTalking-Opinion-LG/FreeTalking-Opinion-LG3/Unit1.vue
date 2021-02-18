<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://i.ytimg.com/vi/D_WS5x4Tjss/hqdefault.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">K-Pop Versus American Pop
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
      <td class = "uppertable" ><b>Henry :</b></td>
      <td class = "lowertable" >We can’t deny the fact that K-pop is all the rage these days. K-pop artists are constantly breaking records on YouTube and topping international music charts. In fact, nine out of the 20 most-viewed online videos in the first 24 hours are K-pop music videos. Unsurprisingly, BTS appears on the list five times. In addition, even without any overseas promotions, K-pop artists are almost always on Billboard and iTunes charts around the world. For instance, Suga’s “Daechwita” entered Billboard through the power of BTS fans. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >American pop is better than K-pop for a number of reasons. First of all, American pop singers are more likely to write their own music. Lady Gaga, for example, usually writes her own songs. She wrote hits like “Bad Romance,” “Paparazzi,” and “Telephone.” Most K-pop singers, especially idols, don’t write any of their music. They simply sing what they are told to sing and flaunt their pretty faces on stage. The goal of K-pop is to make money, so there are separate writers who do all the work.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>pinnacle</b> 절정
        </p>
        <p>
          <b>be all the rage</b> 엄청나게 유행하다
        </p>
        <p>
          <b>overseas</b> 해외의
        </p>
        <p>
          <b>flaunt</b> 과시하다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >요즘 케이팝이 엄청나게 유행한다는 사실을 부정할 수는 없습니다. 케이팝 아티스트들은 유튜브에서 끊임없이 기록을 경신하고 있으며, 국제 음악 차트에서 1위를 차지하고 있습니다. 실제로 처음 24 시간 동안 가장 많이 본 20 개의 온라인 동영상 중 9 개가 케이팝 뮤직 비디오입니다. 아니나 다를까, 방탄소년단이 5번이나 리스트에 등장합니다. 게다가 해외 프로모션이 전혀 없어도 전 세계 빌보드와 아이튠즈 차트에 케이팝 아티스트들이 거의 항상 오르고 있습니다. 예를 들어, 슈가 '대취타'는 방탄소년단 팬들의 힘으로 빌보드에 진출했습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >미국 팝이 케이팝 보다 더 좋은 이유는 여러 가지가 있습니다. 우선, 미국의 팝 가수들은 그들만의 음악을 작곡할 가능성이 더 높습니다. 예를 들어 레이디 가가는 보통 자신의 노래를 씁니다. 그녀는 "배드 로맨스," "파파라치," 그리고 "텔레폰"와 같은 히트곡을 썼습니다” 대부분의 케이팝 가수들, 특히 아이돌들은 그들의 음악을 전혀 쓰지 않습니다. 그들은 그저 노래를 부르라고 시키는 대로 부르고 무대에서 예쁜 얼굴을 자랑합니다. 케이팝의 목표는 돈을 버는 것이기 때문에 모든 일을 하는 작가들이 따로 있습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What is the difference between K-Pop and American Pop?</li>
          <li>What is your favorite K-Pop and American Pop band or group?</li>
          <li>Have you ever been to a K-Pop/American band concert? If yes, how was your experience?</li>
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
