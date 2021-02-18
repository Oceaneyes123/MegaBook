<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://static01.nyt.com/images/2017/04/30/pageoneplus/25A3_conversation/flyingcar1-videoSixteenByNineJumbo1600-v2.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Will Flying Cars Ever Exist?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div style="line-top-opinion1">
  </div>

  <h3  class = "lower-header-opinion1 white--text">Topic</h3>
  <div style = "line-height: 1.6;">
    <div style="padding : 16px;">   

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>Jane :</b></td>
      <td class = "lowertable" >People have been dreaming about flying cars since the 1920s. So many technological advancements have been made since then, but there are still no flying cars! It’s time to let this silly dream go.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Companies such as Airbus and Boeing have confirmed their “airborne vehicles” will be commercially released within the next few years. Uber said they’re working on a flying taxi service and doing test runs next year. We’re almost there!</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>technological</b> 과학 기술의 
        </p>
        <p>
          <b>advancement</b> 발전 
        </p>
        <p>
          <b>silly</b> 어리석은 
        </p>
        <p>
          <b>confirm</b> 사실임을 보여주다 
        </p>
        <p>
          <b>airborne</b> 하늘에 떠 있는 
        </p>
        <p>
          <b>vehicle</b> 차량 
        </p>
        <p>
          <b>commercially</b> 상업적으로 
        </p>
        <p>
          <b>release</b> 공개하다 
        </p>
        <p>
          <b>within</b> 이내에 
        </p>
        <p>
          <b>test run</b> 시운전
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >사람들은 1920년 이후로 하늘을 나는 차에 대해서 꿈을 꿔왔어. 그 이후로 많은 기술 발전이 이루어졌지만 여전히 하늘을 나는 차는 없어! 이제 어리석은 꿈을 버릴 때야.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >에어버스 및 보잉과 같은 회사는 향후 몇 년 내에 "비행 중인 차량"이 상용화 될 것이라고 확정했어. 우버는 하늘을 나는 택시 서비스를 개발하고 있으며 내년에 시운전을 할 것이라고 밝혔어. 거의 다 왔어!</td>
          </tr>
      
          </table>


      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you drive? If yes, do you like driving? Why?
         </li>
         <li>If not, would you like to learn how to drive? Why?</li>
        <li>Do you think flying cars will be common in the future? What would be the advantages and disadvantage</li>
        <li>Would you like to drive a flying car? Why or why not?
      </li>
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
