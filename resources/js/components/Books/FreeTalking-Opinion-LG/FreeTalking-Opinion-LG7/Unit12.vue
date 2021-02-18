<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/healthy-vegetarian-balanced-food-concept-fresh-vegetable-salad-buddha-bowl_114579-7127.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Are Carbs Bad for You?
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
      <td class = "lowertable" >Are carbohydrates unhealthy? Well, I can’t give you a simple yes-or-no answer. The truth is that there are good carbs and bad carbs, just like how there are different types of fats and proteins. Good carbs, such as whole grains, beans, fruits, and vegetables, provide you with vitamins, minerals, fiber, and many other nutrients. Examples of bad carbs include white bread, sugary soda, and pastries. Also, carbs are the most important source of energy for your body, so cutting them out completely is not recommended. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >We’ve been led to believe that our bodies need carbohydrates to function properly. Carb-heavy diets are actually pretty recent. When we were hunter-gatherers, we didn’t have bread or pasta. We survived on meat and plants. According to The Huffington Post, “Humans are not meant to consume an abundant amount of carbohydrates. Unlike protein and fat, carbohydrates supply none of the elements necessary to build or repair tissue in the body.” We should all go on a low-carb diet, like keto, and nourish our bodies with better food.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>function</b> (제대로) 기능하다[작용하다]
        </p>
        <p>
          <b>hunter-gatherer</b> 수렵·채집인
        </p>
        <p>
          <b>abundant</b> 풍부한
        </p>
        <p>
          <b>nourish</b> 영양분을 공급하다
        </p>
         
 
 
 

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >탄수화물은 건강에 해로울까요? 글쎄요, 간단히 예, 아니오로 대답할 수는 없습니다. 사실, 다른 종류의 지방과 단백질이 있는 것처럼 좋은 탄수화물과 나쁜 탄수화물이 있다는 것입니다. 통곡물, 콩, 과일 및 채소와 같은 좋은 탄수화물은 비타민, 미네랄, 섬유질 및 기타 많은 영양소를 제공합니다. 나쁜 탄수화물의 예로는 흰 빵, 설탕이 든 소다, 그리고 페이스트리가 있습니다. 또한 탄수화물은 신체에 가장 중요한 에너지 원이므로 완전히 차단하는 것은 권장되지 않습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >우리는 우리 몸이 제대로 기능하기 위해서는 탄수화물이 필요하다고 믿어왔습니다. 탄수화물 과다 섭취는 사실 꽤 최근의 일입니다. 우리가 수렵 채집가였을 때, 우리는 빵이나 파스타를 먹지 않았습니다. 우리는 고기와 식물로 살았습니다. 허핑턴 포스트(Huffington Post)에 따르면,“인간은 다량의 탄수화물을 섭취하는 것이 아닙니다 단백질과 지방과 달리 탄수화물은 체내의 조직을 형성하거나 회복하는 데 필요한 원소를 전혀 공급하지 않습니다." 우리 모두는 키토와 같은 저탄수화물 식단을 해야 하고, 더 좋은 음식으로 우리 몸에 영양을 공급해야 합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like eating food rich in carbohydrates?</li>
          <li>Do you think carbohydrates are unhealthy?</li>
          <li>Can you go on a day without eating anything that contains carbohydrates?</li>
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
