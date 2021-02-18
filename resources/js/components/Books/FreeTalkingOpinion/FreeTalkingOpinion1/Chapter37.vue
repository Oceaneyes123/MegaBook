<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/top-view-vegan-lettering-made-out-vegetables-white-background_23-2148290829.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Does Veganism Really Help the Environment?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class="line-top-opinion1">
  </div>

  <h3  class = "lower-header-opinion1 white--text">Topic</h3>
  <div style = "line-height: 1.6;">
    <div style="padding : 16px;">   

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>Jane :</b></td>
      <td class = "lowertable" >How are vegans helping the world by having plant-based diets? Their efforts are useless against millions who continue to eat meat. Veganism is just a health fad that makes people feel like special environmentalists!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Experts say veganism may be the best way to reduce an individual’s environmental impact. A person’s carbon footprint from food can be reduced significantly by cutting out animal products. An individual’s efforts help in the long run.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>plant-based</b> 식물성의 
        </p>
        <p>
          <b>effor</b> 노력
        </p>
        <p>
          <b>useless</b> 소용없는 
        </p>
        <p>
          <b>fad</b> 유행
        </p>
        <p>
          <b>environmentalist</b> 환경 운동가 
        </p>
        <p>
          <b>expert</b> 전문가 
        </p>
        <p>
          <b>reduce</b> 줄이다 
        </p>
        <p>
          <b>individual</b> 개인 
        </p>
        <p>
          <b>impact</b> 영향 
        </p>
        <p>
          <b>carbon footprint</b> 탄소 발자국 
        </p>
        <p>
          <b>significantly</b> 상당히 
        </p>
        <p>
          <b>long run</b> 장기간
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >고양이나 개와 달리, 파충류나 양서류 같은 대부분의 이국적인 동물들은 손이 많이 안가. 그래서 그들은 바쁜 사람들에게 완벽해. 파충류와 양서류는 또한 털과 깃털에 알레르기가 있는 사람들에게 좋아!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >멸종 위기에 처해 있거나 포식자인 이국적인 동물들은 애완동물로 받아들여져서는 안 되지만, 많은 사람들은 여전히 불법으로 그것들을 소유해. 그런 동물들을 소유하는 것은 해를 끼치고 질병을 퍼뜨릴 수 있어.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you know anyone who is a vegan?</li>
          <li>What do you think about being a vegan?</li>
          <li>Can you live as a vegan? Why or why not?</li>
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

p{

  margin-top: 10px;
}

h3{
  padding-top: 7px;

}


body{

  font-size: 16px;
}



</style>
