<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/overhead-view-wooden-spoons-with-pills-isolated-white-background_23-2147883817.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should People Bathe Every Day?</h1>
      </transition>
    </v-layout>
  </v-img>

  <div class="line-top-opinion1">
  </div>

  <h3  class = "lower-header-opinion1">Topic</h3>
  <div style = "line-height: 1.6;">
    <div style="padding : 16px;">   

    <table style = "border-collapse: collapse;">

    <tr>
      <td class = "uppertable" ><b>Jane :</b></td>
      <td class = "lowertable" >People need to bathe every day, especially in the summer. The smell of body odor is repulsive! It’s better to feel fresh, clean, and smell nice than to be dirty and stinky.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Studies have shown daily showers are not good. People irritate and dry out their skin from constant washing. They could also be removing helpful bacteria that helps skin stay healthy.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>odor</b> 냄새
        </p>
        <p>
          <b>repulsive</b> 역겨운 
        </p>
        <p>
          <b>fresh</b> 상쾌한 
        </p>
        <p>
          <b>dirty</b> 더러운 
        </p>
        <p>
          <b>stinky</b> 악취가 나는 
        </p>
        <p>
          <b>irritate</b> 자극하다 
        </p>
        <p>
          <b>constant</b> 끊임없는 
        </p>
        <p>
          <b>remove</b> 없애다 
        </p>
        <p>
          <b>helpful</b> 도움이 되는 
        </p>
        <p>
          <b>bacteria</b> 세균
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">


        <table style = "border-collapse: collapse;">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">사람들은 특히 여름에 매일 목욕을 해야 해 체취 냄새가 역겨워! 더럽고 악취가 나는 것보다는 신선하고 깨끗하며 좋은 냄새가 나는 것이 좋아.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">매일 샤워하는 것이 좋지 않다는 연구 결과가 있어. 사람들은 끊임없는 씻는 것을 통해 피부를 자극하고 건조시켜. 또한 피부를 건강하게 하는 데 도움이 되는 박테리아를 제거할 수도 있어.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you agree with Jane or Tom? Why?</li>
          <li>What is your grooming ritual? Do you take a bath before you go out or after going home?</li>
          <li>How important is personal hygiene?</li>
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
