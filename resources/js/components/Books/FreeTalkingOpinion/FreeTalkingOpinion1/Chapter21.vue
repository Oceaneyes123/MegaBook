<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/circle-trash-with-recycle-symbol_23-2147852545.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should Recycling Be Mandatory?
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
      <td class = "uppertable" ><b>A :</b></td>
      <td class = "lowertable" >Recycling is such a hassle! Why should the law require us to do such tedious work?
      People who recycle can receive awards, but you shouldn't force others to do it, too.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>B :</b></td>
      <td class = "lowertable" >Our planet is in a state of crisis due to the environment.
      We cannot be lenient with eco-friendly laws.
      Recycling should be required by law because everyone needs to help reduce pollution.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>Mandatory</b> 법에 정해진
        </p>
        <p>
          <b>hassle</b> 귀찮은 일
        </p>
        <p>
          <b>require</b> 요구하다
        </p>
        <p>
          <b>tedious</b> 지루한
        </p>
        <p>
          <b>award</b> 보상
        </p>
        <p>
          <b>force</b> 강요하다
        </p>
        <p>
          <b>crisis</b> 위기
        </p>
        <p>
          <b>environment</b> 환경
        </p>
        <p>
          <b>lenient</b> 관대한
        </p>
        <p>
          <b>eco-friendly</b> 친환경적인
        </p>
        <p>
          <b>pollution</b> 오염
        </p>
        <br />
        <p style="color: #56AAFF;">
          <b>Be in a state of ~ 의 상태에 있다.</b>
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

                      <p class = "korean">
                        <b>
                        재활용은 법으로 요구되어야 하나요?
                        </b>
                      </p>

                      <table class = "standard-table">

                       <tr>
                        <td class = "uppertable" ><b>A :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >재활용은 정말 번거로워! 법이 왜 우리에게 그렇게 지루한 일을 하라고 요구해야 하는 거야?
                          재활용을 하는 사람들은 상을 받을 수 있지만, 다른 사람들에게도 그것을 하도록 강요해서는 안되지.</td>
                      </tr>
                      <tr style="color:#1565C0;">
                        <td class = "uppertable" ><b>B :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >우리 지구는 환경 때문에 위기에 처해 있어 우리는 친환경 법에 관대할 수 없어.
                          재활용은 법에 의해 요구되어야 하는데, 왜냐하면 모든 사람들은 오염을 줄이는데 도움을 줘야 하기 때문이야.</td>
                      </tr>

                    
                      </table>

        

      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Why do you think recycling should be mandatory?</li>
          <li>How is your government managing the garbage recycling in your country?</li>
          <li>What is your opinion about countries throwing their trash on other nation's territory?</li>
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
