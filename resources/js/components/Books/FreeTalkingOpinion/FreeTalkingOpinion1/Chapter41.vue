<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://i.pinimg.com/originals/e1/50/a2/e150a259560639315f9ecb337ac541ef.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is Writing in Print Better Than Cursive?
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
      <td class = "lowertable" >Writing in cursive is annoying and useless. Learning it was so challenging and pointless. I never write in cursive unless it’s for my signature. Reading cursive handwriting is almost impossible, too!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Cursive is convenient. As students, we need to know how to quickly take notes by hand. After you master the style, writing in cursive is significantly faster than writing in print.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>annoying</b> 짜증스러운 
        </p>
        <p>
          <b>useless</b> 쓸모 없는 
        </p>
        <p>
          <b>challenging</b> 도전적인 
        </p>
        <p>
          <b>pointless</b> 무의미한
        </p>
        <p>
          <b>signature</b> 서명 
        </p>
        <p>
          <b>handwriting</b> 손글씨 
        </p>
        <p>
          <b>impossible</b> 불가능한 
        </p>
        <p>
          <b>convenient</b> 편리한 
        </p>
        <p>
          <b>take notes</b> 필기를 하다 
        </p>
        <p>
          <b>master</b> 완전히 익히다 
        </p>
        <p>
          <b>significantly</b> 상당히
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >필기체로 쓰는 건 짜증나고 쓸모 없어 그것을 배우는 것은 매우 도전적이고 무의미했어 난 서명이 아닌 이상 필기체로 쓰지 않아. 필기체를 읽는 것도 거의 불가능해!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >필기체는 편리해. 학생으로서 우리는 손으로 빠르게 필기 하는 방법을 알아야 하지. 문체를 숙달한 후에 필기체로 쓰는 것이 인쇄체로 쓰는 것보다 상당히 빨라.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you know how to write in cursive? When did you learn it?</li>
          <li>If not, do you think it’s an important skill to learn? Why or why not?</li>
          <li>Which do you prefer, writing or typing? Why?</li>
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
