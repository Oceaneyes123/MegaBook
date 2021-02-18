<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/quinoa-mushrooms-lettuce-red-cabbage-spinach-cucumbers-tomatoes-bowl-buddha-dark-top-view_127032-1963.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should People Become Vegetarian?
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
      <td class = "lowertable" >Vegetarians have been proven to live longer. In a study from 2012, researchers discovered that eating red meat was linked to an increased risk of death from cancer and heart disease. In addition, another study found that switching to a vegetarian diet or just a diet that was very low in meat can increase someone’s life expectancy by 3.6 years. Plus, meat eaters tend to be overweight. According to an Oxford University study, meat eaters are about 2 percent more likely to be obese compared to vegetarians.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Eating meat is not cruel. Vegetarians often say that it is unethical to eat meat, but they ignore the fact that plants are also living things. Research shows that plants actually respond to threats and may even feel fear. Living things die, and that’s just how life is. It’s just how nature works. Moreover, eating meat has been a part of our lives for millions of years. Meat includes tons of protein and other nutrients, and this is one reason why our brains are so developed. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>according</b> ~에 따라서
        </p>
        <p>
          <b>average</b> 평균의
        </p>
        <p>
          <b>link</b> 관련되다
        </p>
        <p>
          <b>expectancy</b> 기대
        </p>
        <p>
          <b>obese</b> 비대한
        </p>
        <p>
          <b>nutrient</b> 영양소
        </p>


      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >채식주의자들이 더 오래 산다는 것이 입증되었습니다. 연구자들은 2012년 연구에서 붉은 고기를 먹는 것이 암과 심장병으로 인한 사망 위험 증가와 관련이 있음을 발견했습니다. 또한 다른 연구에 따르면 채식 식단으로 바꾸거나 고기가 적은 식단이 평균 수명을 3.6년까지 늘릴 수 있다고 합니다. 더욱이 육식주의자들은 과체중이 되는 경향이 있다. 옥스포드 대학의 한 연구에 따르면 육식주의자들은 채식주의자들에 비해 비만이 될 가능성이 2퍼센트 정도 높습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >고기를 먹는 것은 잔인하지 않습니다. 채식주의자들은 종종 고기를 먹는 것이 비윤리적이라고 말하지만, 그들은 식물도 살아있는 것이라는 사실을 무시합니다. 연구에 따르면 식물은 실제로 위협에 대처하고 심지어 두려움을 느낄 수 있습니다. 살아있는 것들은 죽고, 그것은 삶의 방식일 뿐입니다. 그것은 자연의 법칙일 뿐입니다. 더욱이 고기를 먹는 것은 수 백 만년 동안 우리 삶의 일부였다. 고기에는 수많은 단백질과 다른 영양소가 들어 있는데, 이것이 우리의 두뇌가 그렇게 발달된 이유 중 하나입니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Are you a vegetarian? If not, have you considered becoming one?</li>
          <li>Why do you think other people become vegetarians?</li>
          <li>Do you believe that vegetarians are healthier than those who are not? Why or why not?</li>
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
