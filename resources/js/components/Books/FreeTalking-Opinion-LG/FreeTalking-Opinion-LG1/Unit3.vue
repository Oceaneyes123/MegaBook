<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/groom-putting-ring-bride-s-finger_1157-338.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-lg">[08/12] How Important Is Marriage in Today’s Society?
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
      <td class = "lowertable" >Marriage is still important. Being busy is an excuse in our modern world. When people are in love, they want a special bond that forever ties them together. That’s marriage!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >A person may fall out of love. Today’s society generally accepts that people change and move on. No one should feel pressured to marry or stay in a marriage that will leave them unhappy.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>busy</b> 바쁜 
        </p>
        <p>
          <b>excuse</b> 변명 
        </p>
        <p>
          <b>modern</b> 현대의
        </p>
        <p>
          <b>bond</b> 유대
        </p>
        <p>
          <b>fall out</b> 떨어지다 
        </p>
        <p>
          <b>generally</b> 대부분의 사람들이 
        </p>
        <p>
          <b>accept</b> 받아들이다 
        </p>
        <p>
          <b>move on</b> 넘어가다 
        </p>
        <p>
          <b>pressured</b> 부담되는 
        </p>
        <p>
          <b>unhappy</b> 불행한
        </p>

      </div>

      <div class = "line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >결혼은 여전히 중요해. 바쁘다는 것은 우리 현대 사회의 핑계야. 사람들은 사랑에 빠졌을 때 그들을 영원히 함께 묶는 특별한 유대감을 원하지. 그게 결혼이야!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >사람은 사랑이 식을 수도 있어. 오늘날의 사회는 일반적으로 사람들이 변화하고 나아가고 있다는 것을 받아들여. 아무도 결혼하거나 불행하게 될 결혼 생활을 해야 한다는 압박감을 느껴서는 안 되지.</td>
          </tr>
      
          </table>


      </div>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What do you think is the best age to get married? Why?</li>
          <li>Do you think getting married is important? Why or why not?</li>
          <li>What are the common reasons why some people do not want to get married?</li>
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
