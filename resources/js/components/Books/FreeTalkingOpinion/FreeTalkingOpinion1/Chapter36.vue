<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://c0.wallpaperflare.com/preview/121/772/966/lord-of-the-rings-bookshelf-books-red-book.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should Posthumous Works Be Allowed?
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
      <td class = "lowertable" >After writer J. R. R. Tolkien died, his son revised his unfinished writings and published them. Tolkien’s The Silmarillion was released posthumously and has become one of his best works. Without posthumous releases, we would miss out on masterpieces.</td>
    </tr>
    <tr style="color:#1565C0;"> 
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Many posthumous works are released with greedy intentions. Deceased singers like Prince and Michael Jackson have been victims of having their private demos and unused recordings getting released for profit.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>revise</b> 수정하다 
        </p>
        <p>
          <b>unfinished</b> 완성되지 않은 
        </p>
        <p>
          <b>publish</b> 출판하다 
        </p>
        <p>
          <b>miss out</b> 놓치다 
        </p>
        <p>
          <b>masterpiece</b> 명작 
        </p>
        <p>
          <b>greedy</b> 탐욕스러운 
        </p>
        <p>
          <b>intention</b> 의도 
        </p>
        <p>
          <b>deceased</b> 사망한 
        </p>
        <p>
          <b>victim</b> 피해자 
        </p>
        <p>
          <b>private</b> 개인 소유의 
        </p>
        <p>
          <b>recording</b> 녹음 
        </p>
        <p>
          <b>profit</b> 이익
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >작가 J. R. R. 톨킨이 죽은 후, 그의 아들은 미완성의 글을 수정해서 출판했어. 톨킨의 실마릴리언은 사후에 출간되어 그의 최고 작품 중 하나가 되었어. 유작 출간이 없다면, 우리는 걸작을 놓쳤을 거야.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >많은 유작 작품들은 탐욕스러운 의도로 발표돼. 프린스와 마이클 잭슨과 같은 사망한 가수들은 자신들의 사적인 데모와 사용하지 않은 녹음 파일이 이익을 위해 공개되는 희생양이 되어 왔어.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are posthumous works? Can you give an example?</li>
          <li>Is it okay to release posthumous works? Why or why not?</li>
          <li>Whose unreleased work would you like to be released? Why?</li>
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
