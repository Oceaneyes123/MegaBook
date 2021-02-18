<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://1.bp.blogspot.com/-umHGokKFrb0/WdJAZ4Cre1I/AAAAAAAAABM/Irpl2cVZhZEOdb8YSVaq3Ly1CqsyvZqVwCLcBGAs/s1600/conventional-vs-organic-farming-fb.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Organic Food Healthier Than Conventional Food?
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
      <td class = "lowertable" >Countless studies have proven that organic food is healthier than regular food. In 2014, a research paper in the British Journal of Nutrition stated that organic food is higher in nutrients and lower in pesticides than conventionally grown food. The authors reviewed 343 studies to come to this conclusion. Specifically, organic food was found to have more antioxidants. The authors explained, “Many of these compounds have previously been linked to a reduced risk of chronic diseases, including cardiovascular disease and neurodegenerative diseases and certain cancers.”</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Organic food and conventional food are pretty similar in terms of nutrition and health benefits. According to a study done by Stanford University scientists in 2012, “No consistent differences were seen in the vitamin content of organic products.” They concluded that there is no “strong evidence that organic foods are significantly more nutritious than conventional foods.” In 2009, Dr. Alan Dangour, a British nutritionist, published a study stating that organic and non-organic foods are broadly comparable when it comes to nutrients.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>pesticide</b> 살충제, 농약
        </p>
        <p>
          <b>link</b> 관련되다
        </p>
        <p>
          <b>neurodegenerative</b> 신경변성의
        </p>
        <p>
          <b>comparable</b> 비슷한
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >수많은 연구들이 유기농 식품이 일반 식품보다 건강하다는 것을 증명했습니다 2014년, 영국 영양 저널의 한 연구 논문은 유기농 식품이 재래적으로 재배된 식품보다 영양소가 높고 농약이 낮다고 언급했습니다. 저자들은 이 결론에 도달하기 위해 343개의 연구를 검토했습니다. 특히, 유기농 식품은 더 많은 산화 방지제를 가지고 있는 것으로 밝혀졌습니다. 저자들은 "이러한 화합물들 중 다수는 이전에 심혈관 질환과 신경퇴행성 질환, 특정 암을 포함한 만성 질환의 위험 감소와 관련이 있었습니다."라고 설명했습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >유기농 식품과 전통적인 음식은 영양과 건강상의 이점 면에서 상당히 유사합니다. 2012년 스탠포드(Stanford) 대학 과학자들에 의해 행해진 연구에 따르면, "유기 제품의 비타민 함량에서 어떠한 일관된 차이도 발견되지 않았습니다." 그들은 "유기성 식품이 종래의 음식보다 훨씬 더 영양가가 높다는 확실한 증거는 없다"고 결론내렸습니다. 2009년 영국의 영양학자인 앨런 댄거(Alan Dangour) 박사는 유기농 식품과 비 유기농 식품이 영양분에 관한 한 대체로 비슷하다는 연구결과를 발표했습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Which do you consume more? Organic or conventional food? Why?</li>
          <li>What is the difference between organic and conventional food?</li>
          <li>In your opinion, what are the benefits of eating organic food?</li>
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
