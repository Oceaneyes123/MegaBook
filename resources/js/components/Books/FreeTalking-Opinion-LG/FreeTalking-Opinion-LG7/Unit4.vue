<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/high-angle-glasses-with-soft-drink-fruit-juice-with-straws_23-2148691227.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should we just ban soft drinks altogether?
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
      <td class = "lowertable" >The truth is soda is a toxic chemical that people consume on a daily basis! The science has proven that drinking it is bad for you, but people do it anyway. The American Heart Association recommends that men should not eat more than 37.5 g of sugar in one day, with women at 25 g. Just one can of soda goes over the maximum recommendation! And that doesn’t even count the other things you eat every day. Soft drinks must be banned because the consequences are simply not worth it.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >There’s no question that soft drinks contain tons of sugar. And just like everything, too much of one thing is usually bad news. That’s why it’s so important for people to control how much they drink, eat, and consume on a daily basis. Moderation, which means self-control and avoiding excess, is important here. Having a soda every day will hurt you, but what’s wrong with having one every once in a while? In moderation, we can still enjoy a treat like soda with our meals.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>toxic</b> 유독한
        </p>
        <p>
          <b>chemical</b> 화학물
        </p>
        <p>
          <b>recommend</b> 추천하다, 권고하다
        </p>
        <p>
          <b>count</b> 계산에 넣다, 포함시키다
        </p>
        <p>
          <b>control</b> 조절하다
        </p>
        <p>
          <b>consume</b> 섭취하다, 먹다
        </p>
        <p>
          <b>moderation</b> 적당함, 절제
        </p>
  </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >진실은 탄산음료가 사람들이 매일 마시는 독성 화합물이라는 것입니다! 과학이 그것을 마시는 것이 여러분에게 나쁘다는 것을 증명했지만, 사람들은 그래도 그것을 마십니다. 미국심장협회는 남성의 하루 설탕 권장량은 37.5그램이며, 여성은 25그램 이상 먹지 말라고 권고했습니다. 겨우 탄산음료 한 캔이 그 최대 권고량을 넘어갑니다! 그리고 그것은 여러분들이 매일 먹는 다른 음식들은 고려되지 않은 것입니다. 탄산음료는 그 결과를 감수할 만한 가치가 없기 때문에 반드시 금지되어야 합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >탄산음료들이 엄청난 양의 설탕을 함유한다는 것은 반론의 여지가 없습니다. 그리고 다른 모든 것과 같이, 한 가지가 너무 많다면 그것은 보통 나쁜 소식입니다. 그것이 사람들이 매일 그들이 얼마나 마시고, 먹고 섭취하는지 조절하는 것이 매우 중요한 이유입니다. 자기 통제와 과다함을 피한다는 뜻을 가진 절제가 그래서 중요한 것입니다. 매일 탄산음료를 마시는 것은 여러분에게 해로울 테지만, 가끔 한 번씩 마시는 것도 나쁠 것은 없지 않습니까? 절제를 함으로써, 우리는 식사와 함께 탄산음료와 같은 특식을 즐길 수 있게 됩니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you drink soft drinks often?</li>
          <li>Do you think soft drinks can cause health problems? Why or why not?</li>
          <li>In your opinion, should drinking soft drinks be banned?</li>
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
