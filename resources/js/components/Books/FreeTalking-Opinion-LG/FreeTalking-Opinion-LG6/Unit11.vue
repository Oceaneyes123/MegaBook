
<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/side-view-vegetables-with-spices_141793-2612.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Koreans Should Eat Mostly Vegetables
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
      <td class = "lowertable" >In 2015, meat consumption in Korea averaged 51.3 kilograms per capita, more than in China (47.1) and Japan (35.5), a study done by the Organization for Economic Cooperation and Development (OECD) said. Though nowhere near as high as that of the frontrunner U.S. (89.7), Koreans still love to eat red meat such as samgyeopsal and galbi. High consumption of red meat leads to health issues like liver problems, and eating mostly vegetables would solve many ailments like obesity and others caused by meat consumption.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >The human race has done fine with meat consumption. One Time magazine article said humans would’ve never developed their brains without meat. The brain is a demanding organ requiring lots of fuel, and meat provides just that. Plus just about anything eaten in excess causes problems, like Vitamin A. So the key is moderation. Studies have also found no proven health benefits from avoiding meat, while not eating it can cause problems as meat is packed with nutrients like protein. Humans function best when they eat both plants and meat.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>per capita</b> 1 인당
        </p>
        <p>
          <b>frontrunner</b> 선두주자
        </p>
        <p>
          <b>liver</b> 간
        </p>
        <p>
          <b>obesity</b> 비만
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >경제협력개발기구에 의한 연구에 따르면, 2015년 한국의 육류 섭취는 일인당 평균 51.3 킬로그램이며 이는 중국(47.1)과 일본(35.5)보다 많습니다. 선두주자인 미국(89.7)의 섭취량처럼 높지 않지만, 한국인들은 여전히 삼겹살과 갈비와 같은 붉은 고기를 먹는 것을 좋아합니다. 많은 양의 붉은 고기를 섭취하는 것은 간 문제와 같은 건강 문제를 낳으며, 주로 채소 위주의 식사를 하는 것은 비만과 육류 섭취로 인해 발생하는 많은 다른 질병들을 해결할 수 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >인류는 고기 섭취 없이 잘 살아 왔습니다. 타임 매거진의 한 기사는 인간이 고기를 섭취하지 않았다면 뇌를 발전시킬 수 없었을 것이라고 말하였습니다. 뇌는 많은 연료를 요구하는 까다로운 기관이며, 고기를 그것을 제공합니다. 게다가 비타민A와 같이 과도하게 무엇이든 너무 많이 섭취하면 문제를 낳습니다. 따라서 해결책은 절제입니다. 고기가 단백질과 같은 영양소들로 채워져 있기 때문에 그것을 먹지 않는 것은 문제들을 낳을 수 있는 반면, 연구들은 또한 고기를 피하는 것으로부터 오는 검증된 건강상의 이익을 찾지 못하였습니다. 인간은 채소와 고기를 둘 다 먹을 때 가장 잘 기능합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Which do you prefer to eat more? Meat or vegetables? Why?</li>
          <li>Do you agree that Koreans should eat mostly vegetables? Why or why not?</li>
          <li>Do you believe that eating mostly vegetables would solve many ailments? Why or why not?</li>
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
