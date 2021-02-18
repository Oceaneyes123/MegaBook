<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://storage.needpix.com/rsynced_images/lozenge-462867_1280.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-lg">[08/13] Are Cough Drops Unhealthy?
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
      <td class = "lowertable" >The menthol in cough drops is dangerous! An elderly man was taken to the emergency room from menthol poisoning caused by cough drops. Besides, cough drops do not help sore throats to heal.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >The man overdosed from eating two bags of cough drops daily for 20 years. Menthol comes from peppermint oil and is safe in moderation. Also, cough drops are not a treatment. They are meant to give temporary relief.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>dangerous</b> 위험한 
        </p>
        <p>
          <b>elderly</b> 연세가 드신 
        </p>
        <p>
          <b>emergency room</b> 응급실 
        </p>
        <p>
          <b>poisoning</b> 중독 
        </p>
        <p>
          <b>sore</b> 따가운 
        </p>
        <p>
          <b>heal</b> 치유되다 
        </p>
        <p>
          <b>overdose</b> 과다 복용하다 
        </p>
        <p>
          <b>moderation</b> 적당함 
        </p>
        <p>
          <b>treatment</b> 치료 
        </p>
        <p>
          <b>temporary</b> 일시적인 
        </p>
        <p>
          <b>relief</b> 안도 
        </p>

      </div>

      <div class = "line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >목캔디에 들어있는 멘톨은 위험해! 한 노인이 목캔디에 의한 멘톨 중독으로 응급실로 실려갔어. 게다가 목캔디는 목이 아픈 것을 낫게 하는데 도움이 되지 않아.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >그 남자는 20년 동안 매일 두 봉지의 목캔디를 과다 복용했어. 멘톨은 페퍼민트 기름에서 나오며 적당하면 안전해 또한 목캔디는 치료가 아니야. 일시적인 안도감을 주기 위한 것이야.</td>
          </tr>
      
          </table>


      </div>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>
            What do you do to relieve sore throat? Is it effective?
          </li>
          <li>Have you ever tried taking cough drops while suffering from a sore throat?</li>
          <li>Do you do self-medication? Why?</li>
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
