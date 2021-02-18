<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://cdn.pixabay.com/photo/2016/12/23/16/49/feng-shui-1927590_960_720.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is Feng Shui Accurate?
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
      <td class = "lowertable" >Feng shui is a bunch of nonsense. Do people really think moving furniture around will suddenly create huge life changes? It is not a science or art, but simply a fad!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Feng shui is thousands of years old. It is very complex and should not be called a trend about moving furniture. Do your research about feng shui and its relation to quantum physics.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>nonsense</b> 말도 안 되는 것 
        </p>
        <p>
          <b>furniture</b> 가구
        </p>
        <p>
          <b>suddenly</b> 갑자기 
        </p>
        <p>
          <b>science</b> 과학
        </p>
        <p>
          <b>fad</b> 유행 
        </p>
        <p>
          <b>complex</b> 복잡한
        </p>
        <p>
          <b>trend</b> 동향, 추세 
        </p>
        <p>
          <b>research</b> 연구 
        </p>
        <p>
          <b>relation</b> 관계 
        </p>
        <p>
          <b>quantum physics</b> 양자 물리학
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >풍수는 말도 안 되는 소리야. 사람들은 정말로 가구를 이리저리 옮기는 것이 갑자기 큰 삶의 변화를 일으킬 거라고 생각하니? 그것은 과학이나 예술이 아니라 단지 유행일 뿐이야!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >풍수는 수천 년 된 거야. 그것은 매우 복잡하고 가구를 옮기는 것에 관한 유행이라고 불려서는 안 돼. 풍수와 양자 물리학의 관계에 대한 조사를 해 봐.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What do you know about Feng Shui?</li>
          <li>Do you apply Feng Shui teachings in your daily life? Why or why not?</li>
          <li>Do you think Feng Shui has a scientific basis? Why or why not?</li>
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
