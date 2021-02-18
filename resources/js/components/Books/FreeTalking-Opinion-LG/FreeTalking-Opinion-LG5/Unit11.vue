<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://ssl-static.libsyn.com/p/assets/e/7/a/8/e7a879decef25042/k-pop.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Are K-pop Idols Good Role Models?
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
      <td class = "lowertable" >K-pop idols can be good role models for teenagers. Because of their fame, K-pop idols have an opportunity to share their personal experience with their fans. They often have similar problems as modern teenagers, like being bullied or struggling to achieve their dreams. They inspire their fans to work hard and never give up. Some idols even scold their fans into good behavior. Apink’s Eunji said she will beat any fan that skips school to go to a fan signing event. Thus, idols can be positive role models.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Teenagers should not look up to K-pop idols because they portray unrealistic expectations of life. They are beautiful, rich, and famous. It might be hard for teenagers to understand such a lifestyle. K-pop idols always look slim, with perfect hair and make-up. Their fans often want to copy their lifestyle. They go on extreme diets, wear lots of make-up, and don’t demonstrate exemplary behavior. Fans feel like they need to look a certain way, and if they fail, they feel bad about themselves. In other words, K-pop idols can be negative examples for teenagers.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>representative</b> 대표자
        </p>
        <p>
          <b>fame</b> 명성
        </p>
        <p>
          <b>bully</b> 놀리다, 못살게 굴다
        </p>
        <p>
          <b>inspire</b> 영감을 주다
        </p>
        <p>
          <b>skip</b> 건너뛰다, 빼먹다
        </p>
        <p>
          <b>positive</b> 긍정적인
        </p>
        <p>
          <b>portray</b> 나타내다, 보여주다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >케이 팝 아이돌들은 십대들에게 좋은 롤모델리 될 수 있습니다. 그들의 명성 때문에 케이팝 아이돌들은 그들의 개인적 경험을 팬들과 나눌 수 있는 기회가 있습니다. 그들은 종종 따돌림을 받거나 꿈을 위해 고군분투하는 것과 같은 현대 십대들과 비슷한 문제를 가지고 있습니다. 그들은 그들의 팬들이 열심히 일하고 절대 포기 하지 않도록 영감을 줍니다. 몇몇 아이돌들은 심지어 그들의 팬들이 좋은 행동을 하도록 팬들을 혼내기도 합니다. 에이핑크의 은지는 그녀는 팬 싸인회에 가기위해 학교를 결석한 어떤 팬들도 혼낼 것이라고 말했습니다. 그래서 아이돌들은 긍정적인 롤모델이 될 수 있습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >십대들은 케이팝 아이돌들을 존경해서는 안되는데 그들은 인생의 비현실적인 기대를 묘사하기 때문입니다. 그들은 아름답고 부자이고 유명합니다. 십대 청소년들이 그러한 생활스타일을 이해하는 것이 힘들수도 있다고 합니다. 케이팝 아이돌들은 항상 날씬하고 완벽한 머리와 화장을 하는 것처럼 보입니다. 그들의 팬들은 자주 아이돌들의 생활 스타일을 따라하기를 원합니다. 그들은 극도의 다이어트를 하고 많은 화장을 하고 그리고 모범적인 행동을 보이지 않습니다. 팬들은 그들이 어떤 방식으로 보일 필요가 있는 것같이 느껴서 자신들에 대해서 좋지 않게 느낍니다. 다른 말로 하자면 케이팝 아이돌들은 십대들에게 부정적인 본보기가 될 수 있습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Is there a K-Pop idol that you look up to? If yes, who is he/she? If there is none, who do you look up to? Why?</li>
          <li>What traits should a good role model possess?</li>
          <li>Do you agree that K-Pop idols are good role models? Why or Why not?</li>
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
