<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/top-view-black-cutlery-slate_23-2148461729.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Forks Versus Chopsticks
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
      <td class = "lowertable" >Isn’t it obvious that forks are better than chopsticks? Forks are so much easier to use! To use a fork, you simply hold it and stab your food with it. Chopsticks, however, require an uncomfortable holding position. There are even many people of Asian descent who have trouble using them. In addition, chopsticks are extremely unsafe. Many infants have choked on chopsticks, and one woman in China had her eye jabbed with a chopstick. Luckily, she survived. However, her eye is now permanently damaged. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Although it takes some time to learn how to use chopsticks, they are actually more practical than forks. Chopsticks are mainly used to pick things up to eat. However, they can also be used to pick up ingredients without puncturing them. Chopsticks are commonly used in professional kitchens to stir noodles and mixtures. Moreover, wooden chopsticks can be used in place of sticks when making dishes such as corn dogs and skewered meat. Chopsticks are also cheaper and easier to produce. Therefore, they are much better than forks.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>customary</b> 관례적인
        </p>
        <p>
          <b>utensil</b> (가정에서 사용하는) 기구[도구]
        </p>
        <p>
          <b>obvious</b> 분명한[명백한]
        </p>
        <p>
          <b>stab</b> 찌르다
        </p>
        <p>
          <b>infant</b> 유아
        </p>
        <p>
          <b>choke</b> 숨이 막히다
        </p>
        <p>
          <b>jab</b> 찌르다
        </p>
        <p>
          <b>practical</b> 실용적인
        </p>
        <p>
          <b>puncture</b> 구멍을 내다
        </p>
        <p>
          <b>skewer</b> 꼬챙이를 찌르다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >포크가 젓가락보다 낫다는 것이 분명하지 않습니까? 포크는 사용하기가 훨씬 쉽습니다! 포크를 사용하려면 단순히 포크를 잡고 그것으로 음식을 찌르면 됩니다. 그러나 젓가락은 불편한 잡는 자세가 필요합니다. 심지어 그것을 사용하는 데 어려움을 겪는 많은 아시아계 출신의 사람들도 있습니다 또한 젓가락은 매우 안전하지 않습니다. 많은 유아들이 젓가락에 질식하였고, 중국의 한 여성이 젓가락으로 눈을 찔렀습니다 다행히도 그녀는 살아 남았습니다. 그러나 그녀의 눈은 이제 영구적으로 손상되었습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >젓가락 사용법을 배우는 데는 시간이 좀 걸리지만, 사실 그것들은 포크보다 더 실용적입니다. 젓가락은 주로 먹을 것을 집어 올리는 데 사용됩니다. 그러나 그것은 구멍을 뚫지 않고 재료를 집는 데에도 사용할 수 있습니다. 젓가락은 일반적으로 전문 주방에서 국수와 혼합물을 젓는 데 사용됩니다. 게다가, 나무 젓가락은 콘도그나 고기 꼬치 같은 요리를 만들 때 막대기를 대신해서 사용할 수 있습니다. 젓가락은 또한 더 저렴하고 생산하기 쉽습니다. 따라서 포크보다 훨씬 더 좋습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>How old were you when you first used chopsticks?</li>
          <li>Do you prefer using chopsticks to fork? Why or why not?</li>
          <li>On what foods are forks more practical and comfortable to use?</li>
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
