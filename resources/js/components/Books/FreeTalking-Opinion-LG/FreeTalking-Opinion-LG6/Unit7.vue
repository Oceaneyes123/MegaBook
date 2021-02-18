<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/top-view-fast-food-mix-hamburger-doner-sandwich-chicken-nuggets-rice-vegetable-salad-chicken-sticks-caesar-salad-mushrooms-pizza-chicken-ragout-french-fries-mayo_141793-3997.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Fast Food Be Served In School?
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
      <td class = "lowertable" >Fast food is money. Every fast food restaurant that has become a big chain has taken in a lot of money because it’s quick and it’s delicious. Kids can spend money to buy a meal, get it quickly and get right to their studies or their social life without any issues. With the money, schools can upgrade facilities, improve programs, and enrich the education of students. Kids funding their education with their lunch is a great victory for students and schools.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Fast food is dangerously unhealthy. In the 2004 documentary Super Size Me, a man ate McDonald’s fast food for every meal for a month. By the fifth day, he had gained 4.3 kg. Fast food is a poor choice to feed school children. Studies show that fast food consumption can drop test scores. In a study done by Clinical Pediatrics, children who ate fast food regularly scored 4-5 fewer points per average than a non-fast-food eater.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>chain</b> 일련, 띠(처럼 이어진 것)
        </p>
        <p>
          <b>facility</b> 시설
        </p>
        <p>
          <b>enrich</b> 질을 높이다
        </p>
        <p>
          <b>feed</b> 먹이를 주다
        </p>
        <p>
          <b>consumption</b> 소비
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >패스트푸드는 돈입니다. 큰 체인점이 된 모든 패스트푸드 음식점은 빠르고 맛있기 때문에 많은 돈을 법니다. 아이들은 식사 한 끼를 사고 빨리 그것을 받아서 어떤 문제 없이 그들의 공부나 사회 생활로 바로 돌아가기 위해 돈을 사용할 수 있습니다. 돈으로 학교들은 시설물들과 프로그램들을 향상시키고 학생들의 교육의 질을 높일 수 있습니다. 그들의 점심으로 교육에 기금을 제공하는 아이들은 학생들과 학교에 있어 큰 승리입니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >패스트푸드는 위험할 정도 건강에 좋지 않습니다. 2004년 다큐멘터리 슈퍼 사이즈 미에서, 한 남자가 한 달 동안 매끼를 맥도날드의 패스트푸드를 먹었습니다. 다섯 째날, 그는 4.3kg이 쪘습니다. 패스트푸드는 학생들을 먹이는 형편 없는 선택입니다. 연구들은 패스트푸드 섭취가 시험 성적을 떨어트릴 수 있다고 보여줍니다. 임상 소아학에 의해 실시된 연구에 따르면, 정기적으로 패스트푸드를 먹는 어린이들은 패스트푸드를 먹지 않는 아이들에 비해 평균적으로 4-5점 적게 성적을 얻는다고 합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you think that serving fast food in school cafeterias is a bad idea? Why or why not?</li>
          <li>What do you think would happen to a person who frequently eats fast food?</li>
          <li>In your opinion, what is the most ideal meal that a child should eat?</li>
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
