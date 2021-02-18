<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/christmas-composition-gifts-fir-tree-branches-red-decorations-white-wall-winter-new-year-concept-flat-lay-isometric-space-text_169016-1651.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-lg">[08/14] Should Christmas Presents Be Mandatory?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class="line-top-lg">
  </div>

  <h3  class = "lower-header-lg white--text">Topic</h3>
  <div style = "padding : 16px; line-height: 1.6;">

    <table style = "border-collapse: collapse;">

    <tr>
      <td class = "uppertable" ><b>Jane :</b></td>
      <td class = "lowertable" >Regardless of religion, Christmas is a globally recognized holiday. Everyone knows that giving and getting gifts during Christmas is a big tradition. Also, giving Christmas gifts is common courtesy and should be required!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Showing appreciation and goodwill can be done all throughout the year. It should be done genuinely. No one should feel forced to do so by giving away required gifts during the holidays.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>regardless</b> 상관하지 않고 
        </p>
        <p>
          <b>religion</b> 종교 
        </p>
        <p>
          <b>globally</b> 전세계적으로 
        </p>
        <p>
          <b>recognized</b> 인정된 
        </p>
        <p>
          <b>common courtesy</b> 당연한 예의 
        </p>
        <p>
          <b>required</b> 필수의 
        </p>
        <p>
          <b>appreciation</b> 감사 
        </p>
        <p>
          <b>goodwill</b> 친선 
        </p>
        <p>
          <b>genuinely</b> 진정으로 
        </p>
        <p>
          <b>forced</b> 강요된, 억지로 하는
        </p>

      </div>

      <div class = "line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >종교와 상관없이, 크리스마스는 세계적으로 인정받는 명절이야. 모든 사람들은 크리스마스 동안 선물을 주고 받는 것이 큰 전통이라는 것을 알고 있어. 또한, 크리스마스 선물을 주는 것은 일반적인 예의이고 필수적이어야 해!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >감사와 호의의 표시는 일년 내내 할 수 있어. 진정으로 해야 해. 명절 때 필수적인 선물을 나눠주면서 강요를 해서는 안되지.</td>
          </tr>
      
          </table>


      </div>

       <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>
            Do you give Christmas presents to the people around you? Why or why not?
          </li>
          <li>How do you feel when you get a present?</li>
          <li>Should Christmas presents be mandatory? Why or why not?</li>
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
