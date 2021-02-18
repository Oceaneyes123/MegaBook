<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/casual-girl-using-microwave-heat-cup_23-2147764664.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Microwaves Versus Air Fryers
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
      <td class = "lowertable" >Microwave ovens are perfect for those who don’t have enough time to do anything in the kitchen. According to momdot.com, microwaves “heat and cook the food by employing electromagnetic radiation within the microwave frequency range.” And according to appliancecity.co.uk, “Microwave ovens use the heat from this electromagnetic radiation to heat only the food rather than the whole space inside it.” This technology speeds up cooking time. A snack that needs to be cooked for 10 minutes in the oven may only require around two minutes in the microwave.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Air fryers have had a recent surge in popularity because we are becoming more conscious of our health but still want convenience. According to medicalnewstoday.com, “Since air fryers require a fraction of the oil that deep fryers need, people can have a more healthful meal that has similar flavors and textures.” Microwaves promote unhealthy diets. Microwavable meals, like frozen dinners, are packed with calories, fat, and salt. One Hungry Man meal, for example, contains 940 calories, 63 g of fat, and 1,580 mg of sodium.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>electromagnetic radiation</b> 전자기 복사
        </p>
        <p>
          <b>conscious</b> 의식하는
        </p>
        <p>
          <b>convenience</b> 편의, 편리
        </p>
        <p>
          <b>fraction</b> 일부
        </p>
        <p>
          <b>microwavable</b> 전자레인지로 조리할 수 있는
        </p>
       
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >전자레인지는 부엌에서 아무것도 할 시간이 없는 사람들에게 안성맞춤입니다. momdot.com에 따르면, 전자파는 "전자파 주파수 범위 내에서 전자기 방사선을 이용하여 음식을 가열하고 조리합니다." 그리고 Appliancecity.co.uk에 따르면, "전자레인지는 이 전자기 복사의 열을 사용하여 음식 내부의 전체 공간이 아닌 음식 만 가열합니다." 이 기술은 요리 시간을 단축시킵니다. 오븐에서 10분 동안 조리해야 하는 스낵은 전자레인지에서 2분 정도만 필요로 합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >에어프라이어는 우리가 건강에 대해 더 의식하고 있지만 여전히 편리함을 원하기 때문에 최근 인기가 급증했습니다. medicalnewstoday.com에 따르면, "에어프라이어는 튀김기에 필요한 기름의 일부를 필요로 하기 때문에 사람들은 비슷한 맛과 질감을 가진 더 건강에 좋은 식사를 할 수 있습니다." 전자레인지는 건강에 해로운 식단을 조장합니다. 냉동 저녁 식사와 같은 전자레인지로 조리 할 수 있는 식사는 칼로리, 지방 및 소금으로 가득 차 있습니다. 예를 들어, 배고픈 남자 식사 한끼에는 940칼로리, 63그램의 지방, 1,580밀리그램의 나트륨이 들어있습니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you cook at home? If yes, how often?</li>
          <li>Do you have an airfryer? If none, do you plan on getting one?</li>
          <li>Do you think airfryer is more advantageous compared to a microwave?</li>
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
