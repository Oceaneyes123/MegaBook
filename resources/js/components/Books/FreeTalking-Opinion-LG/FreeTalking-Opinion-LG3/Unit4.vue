<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/glasses-contact-lenses-with-copy-space_23-2148320341.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Glasses Versus Contacts
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
      <td class = "lowertable" >Glasses are much better than contact lenses. First of all, safety is extremely important. Contact lenses are known for being quite damaging. They are breeding grounds for bacteria, causing infections and other serious conditions. One study in the Annals of Emergency Medicine highlighted a case about a teenage girl who slept with her contacts overnight. Unfortunately, she developed an ulcer that scarred her eyes. Jon Femling, the lead author of the study, said sleeping with contacts on is very common but terribly risky.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >When it comes to vision aids, contact lenses are unrivaled. According to allaboutvision.com, “Contacts conform to the curvature of your eye, providing a wider field of view and causing less vision distortions and obstructions than eyeglasses.” When you wear glasses, peripheral vision can be distorted. Glasses also cannot beat contacts when it comes to comfort and convenience. Contacts won’t get in the way when you play sports or exercise. They also won’t fog up in certain weather conditions. Plus, glasses make people look dorky.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>breeding ground</b> 번식지
        </p>
        <p>
          <b>ulcer</b> 궤양
        </p>
        <p>
          <b>scar</b> 흉터를 남기다
        </p>
        <p>
          <b>unrivaled</b> 경쟁자[상대]가 없는, 무적의
        </p>
        <p>
          <b>conform</b> 동형으로 되다
        </p>
        <p>
          <b>curvature</b> 만곡
        </p>
        <p>
          <b>peripheral</b> 주변의
        </p>
        <p>
          <b>fog up</b> 김이 서리다
        </p>
        <p>
          <b>dorky</b> 바보의, 이상한
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >안경이 콘택트렌즈보다 훨씬 좋아요 무엇보다도, 안전은 매우 중요합니다. 콘택트렌즈는 상당히 해로운 것으로 알려져 있습니다. 그들은 박테리아의 번식지이며 감염 및 기타 심각한 상태를 유발합니다. 응급의학 연보에 실린 한 연구는 밤새도록 콘텍트렌즈를 끼고 잠을 잔 십대 소녀에 대한 사례를 부각시켰습니다. 불행히도, 그녀는 그녀의 눈에 상처를 입히는 궤양이 생겼습니다. 이 연구의 주요 저자인 존 페믈링은 콘택트렌즈를 끼고 자는 것은 매우 흔하지만 매우 위험하다고 말했습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >시력 보조기구와 관련하여 콘택트렌즈는 독보적입니다. allaboutvision.com에 따르면, "콘택즈렌즈는 눈의 굴곡에 따라 더 넓은 시야를 제공하고 안경보다 시력 왜곡과 방해를 덜 발생시킵니다." 안경을 쓰면 주변 시력이 왜곡될 수 있습니다. 안경은 또한 편안함과 편리함에 있어서 콘택즈렌즈를 이길 수 없습니다. 스포츠를 하거나 운동을 할 때 콘택즈렌즈가 방해가 되지 않습니다 또한 특정 기상 조건에서 김이 서리지 않습니다. 게다가, 안경은 사람들을 이상하게 보이게 해요. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Which do you prefer to wear, eyeglasses or contact lenses? Why?</li>
          <li>What is your impression of a person who wears eyeglasses?</li>
          <li>Why do people wear eyeglasses?</li>
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
