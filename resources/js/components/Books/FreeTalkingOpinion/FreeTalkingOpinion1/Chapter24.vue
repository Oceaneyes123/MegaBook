<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/halfmoon-betta-fish_1150-7816.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is It Okay to Raise Exotic Animals as Pets?
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
      <td class = "lowertable" >Unlike cats and dogs, most exotic animals, like reptiles and amphibians, are low-maintenance. So they’re perfect for busy people. Reptiles and amphibians are also good for people with allergies to fur and feathers!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Exotic animals that are endangered or predators should not be taken in as pets, but many people still illegally obtain them. Owning such animals can cause harm and spread diseases.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>reptile</b> 파충류
        </p>
        <p>
          <b>amphibian</b> 양서류
        </p>
        <p>
          <b>low-maintenance</b> 손이 많이 안 가는 
        </p>
        <p>
          <b>fur</b> 털 
        </p>
        <p>
          <b>feather</b> 깃털 
        </p>
        <p>
          <b>endangered</b> 멸종 위기에 처한 
        </p>
        <p>
          <b>predator</b> 포식자 
        </p>
        <p>
          <b>illegally</b> 불법적으로 
        </p>
        <p>
          <b>obtain</b> 구하다
        </p>
        <p>
          <b>harm</b> 피해
        </p>
        <p>
          <b>disease</b> 질병
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">


  

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">고양이나 개와 달리, 파충류나 양서류 같은 대부분의 이국적인 동물들은 손이 많이 안가. 그래서 그들은 바쁜 사람들에게 완벽해. 파충류와 양서류는 또한 털과 깃털에 알레르기가 있는 사람들에게 좋아!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">멸종 위기에 처해 있거나 포식자인 이국적인 동물들은 애완동물로 받아들여져서는 안 되지만, 많은 사람들은 여전히 불법으로 그것들을 소유해. 그런 동물들을 소유하는 것은 해를 끼치고 질병을 퍼뜨릴 수 있어.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Is there anyone you know who raises exotic pets?</li>
          <li>What are the most common exotic animals raised as pets in your country?</li>
          <li>Would you like to have an exotic pet? Why or why not?</li>
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
