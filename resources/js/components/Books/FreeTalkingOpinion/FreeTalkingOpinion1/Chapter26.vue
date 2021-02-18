<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://www.ap.org/assets/images/press-releases/2.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Do Celebrities Deserve Special Treatment?
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
      <td class = "lowertable" >Celebrities deserve special treatment. Not everyone can become celebrities. Stars live very unique lives as public figures to entertain and captivate commoners. This kind of responsibility is very stressful.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Celebrities do not deserve better treatment than others. Being famous does not mean you are better than ordinary folks.  All jobs have downsides to them and everyone faces challenges in life.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>unique</b> 특별한 
        </p>
        <p>
          <b>public figure</b> 유명 인사
        </p>
        <p>
          <b>captivate</b> 마음을 사로잡다
        </p>
        <p>
          <b>commoner</b> 평민
        </p>
        <p>
          <b>responsibility</b> 책임
        </p>
        <p>
          <b>ordinary</b> 평범한
        </p>
        <p>
          <b>folk</b> 사람
        </p>
        <p>
          <b>downside</b> 불리한 면
        </p>
        <p>
          <b>face</b> 직면하다
        </p>
        <p>
          <b>challenge</b> 도전
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">


        

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">연예인들은 특별한 대우를 받을 자격이 있어. 모든 사람이 유명인이 될 수 있는 것은 아니야 스타들은 일반인들을 즐겁게 하고 사로잡기 위해 공인으로 매우 독특한 삶을 살아. 이런 종류의 책임은 매우 스트레스가 많아.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">연예인들은 다른 사람들보다 더 나은 대우를 받을 자격이 없어. 유명해진다고 해서 보통 사람들보다 낫다는 뜻은 아니야. 모든 직업은 그들에게 단점을 가지고 있으며 모든 사람들은 삶의 도전 과제에 직면해.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you ever dreamed of becoming a celebrity?</li>
          <li>Which celebrity do you admire or respect? Do you think they deserve special treatment?</li>
          <li>Do celebrities have the responsibility to be role models? Why or why not?</li>
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
