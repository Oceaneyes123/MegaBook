<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/group-kids-friends-arm-around-sitting-together_1150-3907.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should Kids Be Allowed to Vote for the President?
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
      <td class = "lowertable" >A wise singer named Whitney Houston once sang, “I believe the children are our future.” Well, if we’re the future, then we should be able to vote for the president!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >We are the generation that will lead the future, but you can’t ignore the fact we’re still growing and learning. Most of us aren’t knowledgeable about the happenings in politics.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>wise</b> 지혜로운 
        </p>
        <p>
          <b>children</b> 아이들 | (child의 복수)
        </p>
        <p>
          <b>future</b> 미래
        </p>
        <p>
          <b>generation</b> 세대
        </p>
        <p>
          <b>lead</b> 이끌다
        </p>
        <p>
          <b>ignore</b> 무시하다
        </p>
        <p>
          <b>fact</b> 사실
        </p>
        <p>
          <b>grow</b> 자라다
        </p>
        <p>
          <b>learn</b> 배우다
        </p>
        <p>
          <b>knowledgeable</b> 많이 아는
        </p>
        <p>
          <b>happening</b> 사건
        </p>
        <p>
          <b>politics</b> 정치
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

    

        
        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">휘트니 휴스턴(Whitney Houston)이라는 한 현명한 가수가 "나는 아이들이 우리의 미래라고 믿어"라고 노래한 적이 있어. 음, 우리가 미래라면, 우리는 대통령에게 투표할 수 있을 거야!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" style = "word-break: keep-all">우리는 미래를 이끌 세대이지만, 넌 우리가 여전히 성장하고 있고 배우고 있다는 사실을 무시할 수는 없어. 우리들 대부분은 정치에서 일어나는 일에 대해 잘 모르지.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>At what age can people start voting in your country?</li>
          <li>Do you think that is the right age to start participating in the elections? Why or why not?</li>
          <li>Have you ever dreamed of becoming the president of your country? Why or why not?</li>
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
