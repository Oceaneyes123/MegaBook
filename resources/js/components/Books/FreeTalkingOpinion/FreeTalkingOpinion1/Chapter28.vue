<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://hips.hearstapps.com/hmg-prod.s3.amazonaws.com/images/tragus-piercings-social-1566412179.png" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is It Okay for Students to Get Their Ears Pierced?
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
      <td class = "lowertable" >We shouldn’t be allowed to get our ears pierced, because most kids can’t maintain clean, healthy earlobes. All of my friends who got their ears pierced eventually got infections. So gross!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Anyone of any age who gets a body modification should know the responsibility that comes with it. Responsible students should be allowed to freely express themselves through piercings.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>maintain</b> 관리하다
        </p>
        <p>
          <b>earlobe</b> 귓불
        </p>
        <p>
          <b>eventually</b> 결국
        </p>
        <p>
          <b>infection</b> 전염병
        </p>
        <p>
          <b>gross</b> 징그러운
        </p>
        <p>
          <b>modification</b> 개조
        </p>
        <p>
          <b>responsibility</b> 책무, 책임
        </p>
        <p>
          <b>responsible</b> 책임감 있는
        </p>
        <p>
          <b>freely</b> 자유롭게
        </p>
        <p>
          <b>express</b> 표현하다
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">대부분의 아이들이 깨끗하고 건강한 귓볼을 유지할 수 없기 때문에, 우리는 귀를 뚫는 것을 허용해서는 안 돼. 귀를 뚫은 내 친구들은 결국 모두 감염이 되었어. 정말 징그러워! </td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">신체를 개조하는 받는 모든 연령대의 사람들은 그것에 수반되는 책임을 알아야 해. 책임감 있는 학생들은 귀를 뚫는 것을 통해 자유롭게 자신을 표현할 수 있도록 해야 해.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What is the proper dress code at your schools before?</li>
          <li>Was it okay to have a piercing at the schools you’ve attended before?</li>
          <li>What do you think about piercings?</li>
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
