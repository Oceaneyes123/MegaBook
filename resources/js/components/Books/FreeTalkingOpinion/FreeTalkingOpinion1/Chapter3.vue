<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://images.pexels.com/photos/122477/pexels-photo-122477.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should We Push People While Waiting In Line?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class="line-top-opinion1 ">
  </div>

  <h3  class = "lower-header-opinion1 white--text">Topic</h3>
  <div style = "line-height: 1.6;">
    <div style="padding : 16px;">

    <p>
      <b>
      Two People Discuss If They Should Push People While Waiting In Line.
      </b>
    </p>

    <table class="standard-table">

    <tr>
      <td class = "uppertable" ><b>A :</b></td>
      <td class = "lowertable" >This morning was so crazy. I was riding the subway. It was full of people.
      When people started to wait in line to get out, someone pushed me out of the way!
      I couldn't believe it. It ruined my morning!</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>B :</b></td>
      <td class = "lowertable" >That is terrible! Sometimes it is hard to wait patiently in such a busy place,
      but people should still keep public order.</td>
    </tr>

    </table>

    </div>

      <div class="line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>push</b> 밀다
        </p>

        <p>
          <b>in line</b> 일렬로, 일직선으로
        </p>

        <p>
          <b>ride</b> 타다
        </p>

        <p>
          <b>subway</b> 지하철
        </p>

        <p>
          <b>get out</b> 나가다
        </p>

        <p>
          <b>ruin</b> 망치다
        </p>
        <br />
        <p style="color: #56AAFF;">
          <b>public order 공공질서</b>
        </p>

      </div>

      <div class="line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">


                      <p class = "korean">
                        <b>
                        줄 서서 기다릴 때 다른 사람들을 밀어도 될까요?
                        두 명의 사람들이 줄 서서 기다리는 동안 사람들을 밀쳐도 되는지 토론을 합니다.
                        </b>
                      </p>

                      <table class="standard-table">

                       <tr>
                        <td class = "uppertable" ><b>A :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >오늘 아침 정말 짜증났어요. 지하철을 타고 있었어요.
                          지하철이 사람들로 꽉 차 있었습니다. 사람들이 나가기 위해 줄을 서서 기다리기 시작했을 때 누군가가 나를 밀쳐냈습니다!
                          믿을 수가 없었어요. 내 아침을 망쳐버렸습니다.</td>
                      </tr>
                      <tr style="color:#1565C0;">
                        <td class = "uppertable" ><b>B :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >정말 최악이네요! 그렇게 바쁜 장소에서 참을성 있게 기다리는 것은 어려워요.
                          하지만 사람들은 공중질서를 잘 지켜야 합니다.</td>
                      </tr>

                      </table>

        


      </div>
     <div class="line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Why do you think most people feel annoyed while waiting in line?</li>
          <li>How do you entertain yourself while waiting in line?</li>
          <li>Have you ever experienced being pushed by someone while waiting in line? Tell me about it.</li>
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
