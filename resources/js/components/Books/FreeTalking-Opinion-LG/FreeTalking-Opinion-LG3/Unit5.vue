<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/happy-female-friends-sitting-sofa-using-digital-tablet-mobile-phone_23-2148080230.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Every Child Have a Smartphone?
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
      <td class = "lowertable" >Every child who is old enough to know how to use a smartphone should be allowed to have one. First, owning a smartphone makes sure that we stay safe. Smartphones allow us to contact our friends, parents, other family members, and trusted adults. We can call them in case there is an emergency. According to Common Sense Media, an organization that promotes safe technology and media, only 24 percent of children from 8 to 12 years old in the U.S. own a smartphone. This needs to change. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Smartphones are too distracting. Bringing a smartphone to school will make it difficult to focus on schoolwork. In addition, a lot of people keep their eyes glued to their phone, even when they’re walking. Thousands of accidents happen every year due to walking and texting. Plus, smartphones are incredibly expensive. The Samsung Galaxy S10, for instance, costs around $900 (W1 million). Yes, there are cheaper phones available, but most children want the latest and fanciest phones. Their greed forces their parents to make huge financial sacrifices.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>outright</b> 완전히
        </p>
        <p>
          <b>lenient</b> 관대한
        </p>
        <p>
          <b>distracting</b> 마음을 산란케 하는
        </p>
        <p>
          <b>greed</b> 욕심
        </p>
        <p>
          <b>financial</b> 금융[재정]의
        </p>
        <p>
          <b>sacrifice</b> 희생
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >스마트폰 사용법을 알 수 있을 만큼 나이가 많은 모든 아이들에게 스마트폰을 가질 수 있도록 허용해야 합니다 첫째, 스마트폰을 소유하는 것은 우리가 안전하게 지내도록 해줍니다. 스마트폰은 우리가 친구, 부모님, 다른 가족, 그리고 신뢰할 수 있는 어른들에게 연락할 수 있게 해줍니다. 응급 상황에 처했을 경우 연락 할 수 있습니다. 안전한 기술과 미디어를 홍보하는 단체인 커먼 센스 미디어에 따르면, 미국의 8세에서 12세 사이의 어린이들 중 24퍼센트만이 스마트폰을 소유하고 있습니다. 이건 바뀌어야 합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >스마트폰은 너무 산만하게 합니다. 스마트폰을 학교에 가져가는 것은 학교 공부에 집중하는 것을 어렵게 만들 것입니다. 또한 많은 사람들이 걸을 때에도 휴대 전화에서 눈을 떼지 않습니다. 걷기와 문자 메시지로 인해 매년 수천 건의 사고가 발생합니다. 게다가 스마트폰은 엄청나게 비쌉니다. 예를 들어, 삼성 갤럭시 S10의 가격은 약 900달러(100만원)입니다. 네, 더 싼 휴대폰이 있지만, 대부분의 어린이들은 최신의 가장 멋진 휴대폰을 원합니다 그들의 탐욕은 부모에게 막대한 재정적 희생을 강요합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What do you think is the proper age for a child to have a phone? Why?</li>
          <li>Should parents inspect their child’s phone from time to time? Why or why not?</li>
          <li>Do smartphones affect a child’s behavior? If yes, how so?</li>
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
