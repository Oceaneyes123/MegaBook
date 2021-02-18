<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/pair-hands-holding-grocery-bag_23-2148382371.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Takeout Versus Delivery
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
      <td class = "lowertable" >Takeout is definitely better. First of all, you don’t need to pay a delivery fee. There are discounts for takeout, too. Also, as long as you practice social distancing, you don’t need to be afraid of becoming infected. According to the U.S. Food and Drug Administration (FDA), “Currently, there is no evidence of food or food packaging being associated with the transmission of COVID-19.” So there’s no need to be so paranoid about going outside and getting something to go. Just use common sense.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Ordering delivery is the better choice. Not only is it more convenient, it is also safer. Ordering takeout means you have to personally pick up your food from a restaurant. Going to a restaurant exposes you to customers who may be sick. Therefore, you should stay home and order delivery. You don’t even have to greet the delivery man in person because you can tell him to drop your order in front of your door. In fact, many delivery apps, such as Baedal Minjok, recommend this method. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>refrain</b> (특히 하고 싶은 것을) 삼가다
        </p>
        <p>
          <b>opt</b> (~을 하기로 하지 않기로) 택하다
        </p>
        <p>
          <b>transmission</b> 전염
        </p>
        <p>
          <b>paranoid</b> 피해망상적인
        </p>
        <p>
          <b>personally</b> 직접
        </p>
        <p>
          <b>expose</b> 노출시키다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >포장 음식이 확실히 나아요. 우선 배달비는 내지 않아도 됩니다. 포장 음식도 할인이 있어요. 또한, 사회적 거리를 두는 연습을 계속 하는 한, 여러분은 감염되는 것을 두려워할 필요가 없습니다. 미 식품의약국(FDA)에 따르면, "현재, 코로나19 전파와 관련된 식품이나 식품 포장의 증거는 없습니다." 따라서 밖으로 나가서 무엇을 얻는 것에 대해 그렇게 피해망상적일 필요는 없습니다. 그냥 상식적으로 생각하세요. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >배달 주문하는 것이 더 나은 선택입니다. 그것은 더 편리할 뿐만 아니라 더 안전합니다 포장 음식 주문은 식당에서 직접 음식을 가져와야 한다는 의미입니다. 식당에 가면 몸이 아픈 손님들에게 노출됩니다(손님들을 만나게 됩니다). 그러므로 여러분은 집에 있으면서 배달 음식을 시켜야 합니다. 배달원에게 문 앞에서 주문한 것을 놓아 달라고 말할 수 있기 때문에 직접 인사할 필요도 없습니다. 사실 배달의 민족 같은 많은 배달 앱들에서 이 방법을 추천합니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What is your go-to take out restaurant and why?</li>
          <li>Do you think it is safer to have your food delivered to your house? Why or why not?</li>
          <li>What protective items do you bring when going outside?</li>
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
