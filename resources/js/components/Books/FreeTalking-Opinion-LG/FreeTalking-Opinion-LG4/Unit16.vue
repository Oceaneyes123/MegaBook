<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/pretty-girl-embarcing-cat-dog_8353-5284.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Are Cats Better Pets Than Dogs?
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
      <td class = "lowertable" >I prefer cats because they are a lot more self-sufficient compared to dogs. Cats are able to survive on their own if you provide them with these three essential resources: food, water, and a litter box. On the other hand, dogs rely too much on their owners. According to Hungary’s Eotvos Lorand University, dogs depend on humans for affection and protection. Dogs have been domesticated to be “man’s best friends,” but they’re more like babies. People pamper dogs and treat them like their own children.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Dogs are great companions. They are always eager to play with you and can provide hours of joy. With cats, however, you can’t really do much. They’re standoffish, cold, distant, and prefer to keep to themselves. But dogs are sociable and love to play interactively. They’ll catch an object and bring it back to you over and over again. If you throw something at cats, they won’t even bat an eye. They might go after it, but they won’t bring it back to you.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>veterinary</b> 수의과의
        </p>
        <p>
          <b>self-sufficient</b> 자급자족할 수 있는
        </p>
        <p>
          <b>litter</b> 고양이 배변 깔개
        </p>
        <p>
          <b>domesticated</b> 길든
        </p>
        <p>
          <b>pamper</b> 소중히 보살피다
        </p>
        <p>
          <b>standoffish</b> (남에게) 쌀쌀한
        </p>
        <p>
          <b>interactively</b> 쌍방향으로
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >저는 고양이를 더 선호하는데 그것들은 개에 비해서 훨씬 더 자급자족하기 때문입니다. 고양이들은 만약 당신이 이 세가지 필수적인 자원: 음식, 물, 그리고 배변 상자만 제공한다면 그들 스스로 생존할 수 있습니다. 반면 개들은 그들의 주인에게 너무 많이 의존합니다. 헝가리의 에오트보스 로랜드 대학에 따르면 개들은 애정과 보호를 위해 인간에 의존한다고 합니다. 개들은 “사람의 가장 친한 친구”로 길들여졌지만 그들은 더 아기 같습니다. 사람들은 개들을 잘 보살피고 자신의 아이들처럼 대합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >개들은 훌륭한 친구입니다. 그들은 항상 당신과 놀고 싶어하고 몇 시간 동안 기쁨을 줄 수 있습니다. 그러나 고양이들과는 많은 것을 할 수 없습니다. 그들은 쌀쌀맞고, 차갑고, 멀리 떨어져 있으며 혼자 있는 것을 선호한다. 그러나 개들은 사회적이고 상호적으로 노는 것을 좋아합니다. 그들은 사물을 받아서 당신에게 계속 다시 가져다 줍니다. 만약 당신이 고양이들에게 무언가를 던지면 그들은 눈도 깜짝하지 않을 것입니다. 그들은 그 것을 따라갈 수는 있지만 당신에게 그것을 가져다 주지는 않을 것입니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you have a pet? If yes, what kind of pet do you have?</li>
          <li>Which do you think is a better companion? A cat or a dog? Why?</li>
          <li>What do you think future pet owners should consider before adopting??</li>
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
