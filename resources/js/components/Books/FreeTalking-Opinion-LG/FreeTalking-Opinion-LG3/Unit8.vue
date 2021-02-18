<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/front-view-colorful-glasses-cocktail_23-2148454467.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Alcohol Be Banned?
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
      <td class = "lowertable" >Alcohol must be banned. According to the World Health Organization (WHO), there were more than 2 million deaths linked to alcohol worldwide in 2004. Alcohol was also responsible for 5.1 percent of the world’s major diseases in 2012. On the WHO’s official website, it is clearly stated that “the harmful use of alcohol is an important public health problem. It impacts people and societies in many ways.” Plus, the American Liver Foundation says that up to 20 percent of heavy drinkers will develop liver disease.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Alcohol is an integral part of society, so it will be incredibly difficult to ban it. Banning alcohol would actually hurt the economy by putting thousands of people out of work. According to a report from 2007, the global alcoholic beverage market was valued at $970 billion (W1.13 quadrillion). A large percentage of the market was and is still in the hands of local enterprises. Furthermore, many governments around the world raise a lot of revenue thanks to the taxes on alcoholic drinks.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>impact</b> 영향을 주다
        </p>
        <p>
          <b>liver</b> 간
        </p>
        <p>
          <b>integral</b> 없어서는 안 될
        </p>
        <p>
          <b>revenue</b> 수익
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >술은 금지 되어야 합니다. 세계 보건기구 (WHO)에 따르면 2004년에 전 세계적으로 술과 관련된 사망자 수는 2백만 명이 넘었습니다. 술은 또한 2012년에 세계 주요 질병의 5.1%에 대한 책임이 있었습니다. 세계보건기구의 공식 웹사이트에는 "술의 유해한 사용은 중요한 공중 보건 문제입니다. 그것은 여러 면에서 사람들과 사회에 영향을 미칩니다." 게다가, 미국 간 재단에 따르면 최대 20 %의 과음자가 간 질환을 앓게 될 것이라고 합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >술은 사회에서 없어서는 안될 부분이므로 금지하기가 매우 어려울 것입니다. 술을 금지하는 것은 실제로 수천 명의 사람들을 실직시킴으로써 경제에 해를 끼칠 것입니다. 2007년의 한 보고서에 따르면, 세계 알코올성 음료 시장은 9700억 달러(W1130조)로 평가되었습니다. 시장의 많은 부분이 예전에도 그랬고, 여전히 현지 기업의 손에 달려 있습니다. 더욱이 전 세계 많은 정부는 알코올성 음료에 부과되는 세금 덕분에 많은 수입을 올립니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What alcoholic drink do you like the most? Why?</li>
          <li>Who do you like drinking with? Why?</li>
          <li>What would an occasion be like if there was no drinking?</li>
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
