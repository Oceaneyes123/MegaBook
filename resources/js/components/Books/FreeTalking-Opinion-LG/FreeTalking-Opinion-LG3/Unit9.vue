<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/desktop-with-laptop-office-elements_23-2148174122.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Laptops Versus Desktop Computers
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
      <td class = "lowertable" >Laptops are much better than desktops. First of all, they’re lightweight and portable. One of the world’s lightest laptops is the Acer Swift 7, which weighs around 889 g! Even though it is small in size, it packs a punch thanks to its Intel Core i7 processor and powerful memory. Can you imagine carrying around a heavy desktop? According to amazon.com, some gaming desktop computers can weigh as much as 27 kg! Many laptops come with powerful graphics cards that are perfect for gaming. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Desktop computers come with many advantages. If you look at all of the benefits of desktops, you’ll see that they’re better than notebooks. On average, desktops are cheaper than laptops. According to statista.com, the average price of a desktop is $630 (W741,000) in the U.S. According to costhelper.com, “Expect to pay $700 (W824,000) to $1,500 (W1.7 million) for a mid-range laptop.” Even though desktops are cheaper, they usually have better specifications. Laptops that cost as little as desktops are often meant for light internet browsing.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>portable</b> 이동이 쉬운
        </p>
        <p>
          <b>separate</b> 따로 떨어진, 별개의
        </p>
        <p>
          <b>pack a punch</b> 강렬한 효과를 가지다
        </p>
        <p>
          <b>advantage</b> 유리한 점, 이점, 장점
        </p>
        <p>
          <b>mid-range</b> 중간급의
        </p>
        <p>
          <b>specification</b> 사양
        </p>
        <p>
          <b>browse</b> 인터넷을 돌아다니다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >노트북은 데스크탑 보다 훨씬 좋습니다. 우선 가볍고 이동하기가 쉽습니다. 세계에서 가장 가벼운 노트북 중 하나인 Acer Swift 7의 무게는 약 889g 입니다. 비록 크기는 작지만 인텔 코어 i7 프로세서와 강력한 메모리 덕분에 강력한 성능을 제공합니다. 무거운 데스크탑을 가지고 다니는 것을 상상할 수 있습니까? amazon.com에 따르면 일부 게임용 데스크탑 컴퓨터의 무게는 27kg까지 나갈 수 있다고 합니다. 많은 노트북에는 게임에 완벽한 강력한 그래픽 카드가 함께 제공됩니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >데스크탑 컴퓨터에는 많은 장점이 있습니다. 데스크탑의 모든 이점을 살펴보면 노트북보다 데스크탑이 더 낫다는 것을 알 수 있습니다. 평균적으로 데스크탑은 노트북보다 저렴합니다. statista.com에 따르면 미국에서 데스크탑의 평균 가격은 630달러 (741,000 원)입니다 costhelper.com에 따르면, “중급 노트북의 경우 700달러 (824,000원)에서 1,500달러 (170 만원)를 지불 할 것으로 예상하십시오.” 데스크탑은 저렴하지만 일반적으로 사양이 더 좋습니다. 데스크탑만큼 저렴한 노트북은 종종 가벼운 인터넷 검색을 위한 것입니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Which one do you own? A laptop or a desktop computer? Why?</li>
          <li>Do you think desktop computers last longer than laptop computers? Why or why not?</li>
          <li>How do you take care of your laptop or computer?</li>
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
