<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://images.saymedia-content.com/.image/t_share/MTc1MTExMDk5MTk5NTMwODIw/top-30-best-historical-korean-dramas-sageuks-you-must-watch.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Are Historical Shows And Films Educational?
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
      <td class = "lowertable" >Films like Braveheart and 300 bring history to life. If it weren’t for these films, the tales of William Wallace and the Spartans of Thermopylae would be kept in dusty history books. These films make history more accessible. History is essentially stories of the past. While events and people are remembered by dates and facts, history is something that must be experienced to truly understand it. Of course, many of these films may not be 100% authentic. However, many of them also have historians and consultants to help ensure accuracy and authenticity.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >While films and TV shows are entertaining, they are far from educational. If we considered movies and TV to have educational content, then films like The Exorcism of Emily Rose or The Ring would be considered true stories. In truth, they are based on true stories and are almost always considered to be myths. Films take stories and make them as entertaining as possible. By using entertainment as education, we may be mistaken in believing that historical figures did things that never happened. A classic example would be William Wallace in Braveheart screaming “Freedom” at the top of his voice while dying.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>entertaining</b> 재미있는, 즐거움을 주는
        </p>
        <p>
          <b>muddle</b> 헝클어뜨리다, 뒤죽박죽을 만들다
        </p>
        <p>
          <b>detrimental</b> 해로운
        </p>
        <p>
          <b>bring ~ to life</b> ~을 활기 넘치게 하다
        </p>
        <p>
          <b>Spartan</b> 스파르타의
        </p>
        <p>
          <b>accessible</b> 접근 가능한
        </p>
        <p>
          <b>essentially</b> 근본적으로
        </p>
        <p>
          <b>authentic</b> 진짜인
        </p>
        <p>
          <b>consultant</b> 상담가
        </p>
        <p>
          <b>accuracy</b> 정확성
        </p>
 
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >브레이브하트와 300 과 같은 영화는 삶에 역사를 가져와줍니다. 만약 이러한 영화들이 없다면 윌리엄 월레이스와 데르모필레의 스파르타의 이야기가 먼지 쌓인 역사책 속에 감춰질 것입니다. 이런 영화들은 역사를 더 접근하기 쉽게 만듭니다. 역사는 과거의 필수적인 이야기 입니다. 물론 이 영화들 중 많은 것들이 100 프로 진짜는 아닙니다. 그러나 이것들 중 많은 것들이 또한 정확성과 사실성을 확실하게 하도록 도와주는 역사학자나 상담자들을 가지고 있습니다.  </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >영화와 티비 드라마가 재미있는 반면에 그것들은 교육적인 것과는 거리가 멉니다. 우리가 교육적인 내용이 있는 영화와 티비를 생각한다면 액소시즘 오브 에미리로즈나 링과 같은 것들이 실화라고 믿어질 수 도 있습니다. 사실, 그것들은 실화를 바탕으로 하고 거의 신화라고 항상 여겨집니다. 영화들은 이야기를 택하고 그 이야기들을 가능한 한 재미있게 만듭니다. 교육으로 오락을 사용하는 것으로 우리는 역사적 인물들이 절대 일어나지 않았던 일들을 했다고 믿는 실수를 할 수 있습니다. 전형적인 예가 브레이브 하트에서 죽어가는 동안 윌리엄 월리스의 “자유”라고 가장 큰 목소리로 외치는 것이 될 수 있습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you watched historical shows? If yes, what are they? If none, do you plan to watch one?</li>
          <li>Do you find historical shows and films effective in educating people? Why or why not?</li>
          <li>Do you think historical shows and films are important? Why or why not?</li>
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
