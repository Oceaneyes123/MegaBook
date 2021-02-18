<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/elegant-woman-brown-coat-with-black-bulldog_1157-31794.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Get Rid Of Pet Cafes?
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
      <td class = "lowertable" >Pet cafes should be banned because they often expose their animals to a filthy, unhygienic environment. Step into any pet cafe and you’ll instantly get hit with a foul odor. One time, I visited a dog cafe in Seoul, and one whiff of the place was enough to knock me out. Although I adore dogs, I was unable to stay for very long. I’ve also visited a cat cafe, and it was like an enormous litter box! I don’t understand why these pet cafes are so dirty.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Gio Cat Cafe lets customers play, feed, and relax with a lot of cats. More importantly, some of the cats are up for adoption. In fact, many pet cafes put their animals up for adoption. Cafe owner Park Tae-hyeon rescues abandoned pets and provides them a warm, cozy place to stay. “I occasionally find motherless puppies when I go out at night,” he says. “The most popular dog at our cafe is Lemon. His previous owner threw him out for being too old.”</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>unhygienic</b> 비위생적인
        </p>
        <p>
          <b>foul</b> 악취 나는
        </p>
        <p>
          <b>odor</b> 악취
        </p>
        <p>
          <b>whiff</b> 훅 끼치는 냄새
        </p>
        <p>
          <b>litter</b> 배변용 깔개
        </p>
        <p>
          <b>rescue</b> 구조하다
        </p>
        <p>
          <b>occasionally</b> 가끔
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >애완 동물 카페는 동물을 더럽고 비 위생적인 환경에 자주 노출시키기 때문에 금지되어야 합니다. 애완 동물 카페에 들어가면 즉시 고약한 냄새가 납니다. 한 번은 제가 서울의 개 카페를 방문했는데 그 곳의 냄새를 한 번 들이마시는 것만으로도 쓰러질 뻔 했습니다. 비록 제가 개를 아주 좋아하지만 아주 오래 머물지는 못했습니다 저는 또한 한 고양이 카페를 방문했는데 그곳은 거대한 애완 동물용 변기 같았습니다! 저는 왜 이 펫 카페들이 그렇게 더러운지 모르겠습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >지오 고양이 카페는 손님들이 고양이와 함께 놀고, 먹이를 주고, 긴장을 풀도록 합니다. 더욱 중요한 것은 그 고양이들 중 몇은 입양을 위해 내놓았습니다. 사실 많은 펫 카페들이 동물들을 입양을 위해 내놓습니다. 카페 주인인 박태현씨는 유기된 애완동물들을 구출해서 그들이 머무를 따뜻하고 안락한 장소를 제공합니다. “저는 밤에 외출할 때 때때로 어미없는 강아지를 발견합니다.”라고 그가 말합니다. “카페에서 가장 인기 있는 개는 레몬입니다. 그 개의 전 주인은 그 개가 너무 늙었다고 그를 버렸습니다.” </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Are pet cafes popular in Korea? Why or why not?</li>
          <li>Have you been to a pet cafe? If yes, how was your experience? If not yet, do you plan on visiting one?</li>
          <li>Do you have a pet? As a pet-owner or a non-pet-owner, what can you say about pet cafes?</li>
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
