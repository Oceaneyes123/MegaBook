<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/top-view-word-with-cigarettes_23-2148160818.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Cigarettes Be Banned?
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
      <td class = "lowertable" >I believe it is necessary to ban tobacco products altogether. Korea has one of the world’s highest daily smoking rates. In recent years, the government has made many efforts to fix this problem. For example, smoking is banned in many places now, and the price of cigarettes has increased as well. But nothing has really changed. In 2015, the daily smoking rate for men was at an astonishing 40.3 percent. The next year, it actually increased. Then it dropped by a measly 2 percent in 2017.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >School uniforms infringe upon students’ right to express their individuality. The U.S. Constitution states that everyoneThere is no need to make cigarettes illegal. Despite what Henry said, Korea’s smoking rates are steadily going down. He failed to mention that the daily smoking rate for men in Korea was as high as 45.6 percent in 2012. It has been decreasing gradually since then, and this is all thanks to the Korean government’s efforts to fix the country’s smoking problem. Instead of banning cigarettes, we should come up with more ways to get people to smoke less, and they will stop eventually.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>lower</b> 낮추다
        </p>
        <p>
          <b>fix</b> 바로잡다, 손보다
        </p>
        <p>
          <b>astonishing</b> 놀라운, 믿기 힘든
        </p>
        <p>
          <b>measly</b> 쥐꼬리만한
        </p>
        <p>
          <b>illegal</b> 불법적인
        </p>
 
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >저는 담배 제품을 모두 금지해야 한다고 생각합니다. 한국은 세계에서 가장 높은 일일 흡연율을 가지고 있습니다. 최근 몇 년간 정부는 이 문제를 고치기 위해 많은 노력을 했습니다. 예를 들어 흡연은 이제 많은 장소에서 금지되었고 담배 가격 또한 상승되었습니다. 그러나 아무것도 사실상 바뀐 것이 없습니다. 2015년에 남성의 일일 흡연율은 놀랍게도 40.3 퍼센트였습니다. 다음해 그것은 사실 증가했습니다. 그리고 나서 흡연율은 2017년에 2 퍼센트 정도로 약간만 떨어졌습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >담배를 불법으로 만들 필요는 없습니다. 핸리가 말한 것에도 불구하고 한국의 흡연율은 꾸준히 떨어지고 있습니다. 그는 한국 남성의 일일 흡연율이 2012년에 45.7 퍼센트만큼 높았다는 것을 언급하지 못했습니다. 그 이후로 흡연율은 점점 감소했고 이것은 국가의 흡연 문제를 고치려는 한국 정부의 노력 덕분입니다. 담배를 금지하는 대신 우리는 사람들이 담배를 덜 피우게 할 더 많은 방법들을 생각해내야 하고, 그들은 결국 담배를 끊을 것입니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you know people who smoke? If yes, why do you think they smoke?</li>
          <li>Do you see smoking as a problem? Why or why not?</li>
          <li>What do you think are the pros and cons of cigarettes being banned?</li>
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
