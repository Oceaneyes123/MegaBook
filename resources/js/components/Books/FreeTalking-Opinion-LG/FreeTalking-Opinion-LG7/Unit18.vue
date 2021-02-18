<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/kiwies-oranges-colorful-bell-peppers_114579-5951.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Fruits Versus Vegetables
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
      <td class = "lowertable" >Fruits and vegetables aren’t nutritionally equivalent. Out of various fruits and vegetables, dried apricots surprisingly come out on top when it comes to fiber. Dried apricots contain more than 7 g of fiber in a serving of 100 g. Fried potatoes and sweet potatoes, however, contain around 3 g each per 100-g serving. Fruits are generally rich in nutrients, and they’re delicious as well. Many vegetables, on the other hand, tend to be bitter and unpleasant in texture. Thus, if you must choose, go with fruits.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Vegetables are better than fruits because they contain less sugar. Sugar is one of the unhealthiest things you can eat. Too much sugar can lead to weight gain, increase your risk of heart disease, cause acne, and put you at risk of developing diabetes. Nutritionist Paula Simpson said, “Some fruits are dense with sugar and lack fiber. These types of fruits are considered ‘high glycemic,’ meaning they are rapidly digested, causing quick spikes in blood sugar and insulin levels.” Therefore, we should all eat more vegetables.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>nutritionally</b> 영양적으로
        </p>
        <p>
          <b>equivalent</b> 동등한
        </p>
        <p>
          <b>apricot</b> 살구
        </p>
        <p>
          <b>tend</b> (~하는) 경향이 있다
        </p>
        <p>
          <b>bitter</b> 맛이 쓴
        </p>
        <p>
          <b>texture</b> 질감
        </p>
        <p>
          <b>acne</b> 여드름
        </p>
        <p>
          <b>glycemic</b> 혈당(증)의
        </p>
        <p>
          <b>digest</b> 소화되다
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >과일과 야채는 영양적으로 동등하지 않습니다. 다양한 과일과 채소 중에서, 섬유질에 관한 한, 건조된 살구는 놀랍게도 최고입니다. 건조된 살구는 100그램에 7그램 이상의 섬유질을 함유하고 있습니다. 하지만, 튀긴 감자와 고구마는 100그램 당 각각 약 3그램을 포함합니다. 과일은 일반적으로 영양소가 풍부하고, 맛도 좋습니다. 반면에, 많은 야채들은 맛이 쓰고 질감이 불쾌한 경향이 있습니다. 그러므로, 여러분이 선택해야 한다면, 과일과 함께 하세요.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >야채는 당분을 적게 함유하고 있기 때문에 과일보다 더 좋습니다. 당분은 여러분이 먹을 수 있는 가장 건강에 좋지 않은 것들 중 하나입니다. 너무 많은 당분은 체중 증가, 심장병 위험 증가, 여드름 유발, 그리고 당뇨병에 걸릴 위험으로 이어질 수 있습니다. 영양학자 폴라 심슨(Paula Simpson)은 "어떤 과일은 당분 밀도가 높고 섬유질이 부족합니다. 이런 종류의 과일은 '고혈당'으로 여겨지는데, 이는 혈당과 인슐린 수치가 빠르게 치솟는 것을 의미합니다." 라고 말하였습니다. 그러므로, 우리는 더 많은 야채를 먹어야 합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like eating fruits and vegetables? Why or why not?</li>
          <li>In your opinion, should we lessen our fruit intake because of it’s sugar content?</li>
          <li>Do you think it’s okay to eat only vegetables and no fruits? Why?</li>
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
