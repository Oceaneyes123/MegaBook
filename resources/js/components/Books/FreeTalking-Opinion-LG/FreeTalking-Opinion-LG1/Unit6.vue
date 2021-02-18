<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/asian-woman-using-alcohol-gel-hand-sanitizer-wash-hand-protect-coronavirus-female-push-alcohol-bottle-clean-hand-hygiene-when-social-distancing-stay-home-self-quarantine-time_7861-2482.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-lg">[08/18] Are Hand Sanitizers Unhealthy?
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
      <td class = "lowertable" >Hand sanitizers make germs stronger! Viruses evolve to counteract ways to stop them. Overusing hand sanitizers helps germs resist antibiotics. Hand sanitizers are actually training germs to hurt us!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >There is no proof that hand sanitizers help germs become resistant. A hand sanitizer should never replace the act of washing your hands. It is for quick cleaning, like in hospitals, or when there are no sinks available. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>germ</b> 세균
        </p>
        <p>
          <b>evolve</b> 발달하다
        </p>
        <p>
          <b>counteract</b> 대응하다 
        </p>
        <p>
          <b>overuse</b> 남용하다 
        </p>
        <p>
          <b>resist</b> 저항하다 
        </p>
        <p>
          <b>antibiotic</b> 항생제 
        </p>
        <p>
          <b>proof</b> 증거 
        </p>
        <p>
          <b>replace</b> 대신하다 
        </p>
        <p>
          <b>available</b> 이용할 수 있는 
        </p>

      </div>

      <div class = "line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >손 세정제는 세균을 더 강하게 만들어! 바이러스는 그들을 멈추게 하는 방법에 대항하기 위해 진화해 손 세정제를 과다하게 사용하면 세균이 항생제에 저항을 하는 것을 도와 손 소독제는 실제로 세균을 훈련시켜 우리를 상하게 해!</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >손 소독제가 세균이 내성을 갖게 하는 데 도움이 된다는 증거는 없어. 손 세정제는 절대로 손을 씻는 행위를 대신해서는 안 되지. 병원이나 세면대가 없는 경우와 같이 빠른 씻기를 위한 것이야.</td>
          </tr>
      
          </table>


      </div>

<div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>
            How important is it to keep your hands clean? Why?
          </li>
          <li>Do you think hand sanitizers are unhealthy? Why or why not?</li>
          <li>How do you keep your hands clean?</li>
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
