<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/little-kids-halloween-party_53876-41151.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should Korea Celebrate Halloween?

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
      <td class = "lowertable" >Isn’t Halloween about celebrating evil? Is that a good message for our youth? I don’t think so! Also, feeling obligated to wear a costume is a hassle. Halloween is such a pointless holiday!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Halloween was originally a religious holiday that honored the dead. Modern festivities like trick-or-treating are nonreligious, so anyone can participate. Kids in Korea deserve a day like Halloween, where they can dress up and have fun.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>celebrate</b> 기념하다
        </p>
        <p>
          <b>evil</b> 악 
        </p>
        <p>
          <b>youth</b> 젊은이 
        </p>
        <p>
          <b>obligated</b> 의무가 있는 
        </p>
        <p>
          <b>costume</b> 복장 
        </p>
        <p>
          <b>hassle</b> 귀찮은 상황 
        </p>
        <p>
          <b>pointless</b> 무의미한 
        </p>
        <p>
          <b>religious</b> 종교의 
        </p>
        <p>
          <b>the dead</b> 죽은 사람 
        </p>
        <p>
          <b>participate</b> 참여하다 
        </p>
        <p>
          <b>deserve</b> 받을 만하다
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >할로윈은 악을 기념하는 것이 아니니? 우리 젊은이들에게 좋은 메시지일까? 나는 그렇게 생각하지 않아! 또한 의상을 입어야 한다는 의무감을 느끼는 것도 번거롭잖아. 할로윈은 무의미한 휴일이야.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >할로윈은 원래 죽은자를 기리는 종교적인 휴일이었어. 트릭 오어 트릿과 같은 현대의 축제는 종교적이지 않으므로 누구나 참여할 수 있어. 한국의 어린이들은 할로윈처럼 옷을 입고 하루를 즐겁게 즐길 만한 자격이 있어.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you ever experienced celebrating Halloween? How was it?</li>
          <li>If not, would you like to experience it? Why or why not?</li>
          <li>How popular is Halloween in Korea?</li>
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
