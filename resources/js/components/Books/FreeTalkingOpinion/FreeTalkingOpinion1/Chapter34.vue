<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/silhouette-human-hand-holding-bible-cross-background-is-sunrise_1150-7211.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is Humility a Virtue?
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
      <td class = "lowertable" >Being humble is unhealthy because it makes you belittle yourself. Why should I soften myself for other People? Humility is a useless trait that makes us weak.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Many people confuse humility with low self-esteem. Being humble means being authentic. It means being honest with yourself and others. Humble people are self-aware and try to see the good in everyone, including themselves.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>belittle</b> 하찮게 만들다
        </p>
        <p>
          <b>soften</b> 약화시키다 
        </p>
        <p>
          <b>useless</b> 쓸모 없는 
        </p>
        <p>
          <b>trait</b> 특성 
        </p>
        <p>
          <b>weak</b> 약한 
        </p>
        <p>
          <b>confuse</b> 혼동하다 
        </p>
        <p>
          <b>self-esteem</b> 자부심 
        </p>
        <p>
          <b>authentic</b> 진정한 
        </p>
        <p>
          <b>honest</b> 정직한 
        </p>
        <p>
          <b>self-aware</b> 자기를 인식하는
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >겸손해지는 것은 자신을 비하하게 하기 때문에 건강에 좋지 않아. 왜 내가 다른 사람들을 위해 나 자신을 약하게 해야 하니? 겸손은 우리를 약하게 만드는 쓸모 없는 특성이야</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >많은 사람들은 겸손과 낮은 자존감을 혼동하지. 겸손하다는 것은 진실한 것을 의미해. 그것은 자신과 다른 사람들에게 솔직하다는 것을 뜻해. 겸손한 사람들은 자각을 하고 자신을 포함한 모든 사람들의 좋은 점을 보려고 노력하지.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What is humility for you?</li>
          <li>Do you think being humble has disadvantages? Why or why not?</li>
          <li>Who is the humblest person you know?</li>
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
