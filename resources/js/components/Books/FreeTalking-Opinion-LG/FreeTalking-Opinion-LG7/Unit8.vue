<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/3d-render-bedroom_1048-8372.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Soft Versus Firm Beds
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
      <td class = "lowertable" >Soft beds are better than firm beds. Why sleep on a firm bed when you can just sleep on the floor? Although comfort is subjective, most people agree that soft beds feel more comfortable than rock-hard beds. According to the U.S. Sleep Foundation, 93 percent of Americans feel that a comfortable bed is important when it comes to sleep quality. Also, soft mattresses are better for couples because they absorb motion better. With firm mattresses, moving around even just a little bit can disturb your partner.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Sleeping on a firm mattress has huge benefits, like giving your body the support it needs. Firm mattresses hold up the body instead of letting it sink in too much. This is good for people with mobility issues. Those who have trouble moving around because of an injury or health problem should choose a firm mattress. Firm mattresses make it easy to switch positions and get in and out of bed. In addition, they’re cooler than soft mattresses, which can trap body heat and make you sweat.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>subjective</b> 주관적인
        </p>
        <p>
          <b>absorb</b> 흡수하다
        </p>
        <p>
          <b>benefits</b> 유익하다
        </p>
        <p>
          <b>support</b> 지지
        </p>
        <p>
          <b>mobility</b> 이동성
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >푹신한 침대가 단단한 침대보다 낫습니다. 바닥에서 그냥 잘 수 있는데 왜 단단한 침대에서 자나요? 비록 편안함이 주관적이지만, 대부분의 사람들은 푹신한 침대가 바위처럼 단단한 침대보다 더 편안함을 느낀다는 것에 동의합니다. 미국 수면 재단에 따르면, 93퍼센트의 미국인들은 수면의 질에 있어서 편안한 침대가 중요하다고 느낀다고 합니다. 또한 푹신한 매트리스는 움직임을 더 잘 흡수하기 때문에 커플들에게 더 좋습니다. 단단한 매트리스를 사용하면 조금만 움직여도 상대방을 방해 할 수 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >단단한 매트리스에서 잠을 자는 것은 여러분의 몸에 필요한 지원을 제공하는 것과 같은 큰 이점이 있습니다. 단단한 매트리스는 몸이 너무 많이 가라 앉게 하지 않고 몸을 받쳐줍니다. 이것은 몸을 움직이는데 문제가 있는 사람들에게 좋습니다. 부상이나 건강상의 문제로 거동이 불편한 사람들은 단단한 매트리스를 선택 해야 합니다.. 단단한 매트리스를 사용하면 쉽게 자세를 바꾸고 침대에 누웠다 나올 수 있습니다. 게다가 당신의 체온에 열을 가해 땀을 흘리게 하는 푹신한 매트리스보다 시원합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you ever tried sleeping on a soft bed? How about a firm bed?</li>
          <li>Which do you think is better to use?</li>
          <li>Do you agree that comfort helps a person have better sleep? Why or why not?</li>
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
