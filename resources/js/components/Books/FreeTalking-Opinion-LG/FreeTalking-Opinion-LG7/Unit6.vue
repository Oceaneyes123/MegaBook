<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/colorful-dessert-mochi_1339-5321.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Bread Versus Rice Cakes
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
      <td class = "lowertable" >Bread is recognized as a staple food in many parts of the world. It is a culturally important food that has been eaten since ancient times. Some experts believe our ancestors began eating bread around 30,000 years ago. Bread is an important part of human history and has even had an impact on religion and politics. Rice cakes only started receiving attention throughout the world after becoming a short-lived trend as a diet food. It is nearly impossible for rice cakes to ever reach the status of bread.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Rice cakes initially received attention in the West after puffy rice crackers were introduced as healthy snacks. Some believe interest in rice cakes died along with the rice cracker fad in the 20th century. However, the versatility of rice cakes is now being recognized as more people are being introduced to other dishes. People in Asia have been enjoying the soft, chewy texture of rice cakes for years. Another positive outcome of globalization is that many countries are discovering the variety of rice cake dishes.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>culturally</b> (한 사회의) 문화와 관련된, 문화의
        </p>
        <p>
          <b>impact</b> 영향
        </p>
        <p>
          <b>versatility</b> 다재, 다예, 다능, 융통성 있음
        </p>
        <p>
          <b>texture</b> (음식이 입 안에서 느껴지는) 질감
        </p>
        <p>
          <b>globalization</b> 세계화
        </p>
 
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >빵은 세계 많은 지역에서 주식으로 인정받고 있습니다. 고대부터 먹어온 문화적으로 중요한 음식입니다. 일부 전문가들은 우리 조상들이 약 30,000년 전에 빵을 먹기 시작했다고 믿고 있습니다. 빵은 인류 역사의 중요한 부분이고 심지어 종교와 정치에 영향을 끼쳤습니다. 떡은 다이어트 식품으로 순식간 유행이 된 후에야 전 세계적으로 주목을 받기 시작했습니다. 떡이 빵의 위치에 도달하는 것은 거의 불가능합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >떡은 처음에 서양에서 푹신한 쌀 과자가 건강에 좋은 간식으로 소개된 후 주목을 받았습니다. 일부는 떡에 대한 관심이 20세기 쌀 과자의 유행과 함께 사라졌다고 믿고 있습니다. 그러나 이제는 더 많은 사람들이 다른 요리를 접하게 되면서 떡의 다양성이 인정 받고 있습니다. 아시아 사람들은 수년간 부드럽고 쫄깃한 떡의 식감을 즐겨왔습니다. 세계화의 또 다른 긍정적인 결과는 많은 나라들이 떡 요리의 다양성을 발견하고 있다는 것입니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like eating bread? What is your favorite?</li>
          <li>How often do you eat rice cake? What is your favorite rice cake dish?</li>
          <li>In your opinion, is rice cake better than bread?</li>
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
