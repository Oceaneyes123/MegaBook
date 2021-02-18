<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/asian-young-happy-family-enjoy-vacation-beach-evening-dad-mom-kid-relax-playing-together-near-sea-when-silhouette-sunset-lifestyle-travel-holiday-vacation-summer-concept_7861-2443.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Is The Korean Age System More Useful Than The Regular Age System?
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
      <td class = "lowertable" >With the Korean age system, it's easier to find out how old someone is.
      You just need to subtract their birth year from the current year and then add one.
      There is no need to calculate months or dates.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>B :</b></td>
      <td class = "lowertable" >Most countries use the regular age system. In fact, counting in the regular age system is more accurate.
      Plus, many medical and government papers ask you to write down your regular age.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>find out</b> 알아내다
        </p>
        <p>
          <b>subtract</b> 빼다
        </p>
        <p>
          <b>current</b> 지금의
        </p>
        <p>
          <b>calculate</b> 계산하다
        </p>
        <p>
          <b>count</b> 수를 세다
        </p>
        <p>
          <b>Regular age system</b> 단나이
        </p>
        <p>
          <b>accurate</b> 정확한
        </p>
        <p>
          <b>medical</b> 의료의..
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">

                      <p class = "korean">
                        <b>
                        한국 나이 시스템이 만 나이 시스템보다 더 유용한가요?
                        </b>
                      </p>

                      <table class = "standard-table">

                       <tr>
                        <td class = "uppertable" ><b>A :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >한국 나이 체계로는,
                          누군가가 몇 살인지 알아내는 게 더 쉬워 너는 바로 그들의 생년월일을 현재 년도에서 빼서 한 해를 더하면 된다.
                          월이나 날짜를 계산할 필요가 없어.</td>
                      </tr>
                      <tr style="color:#1565C0;">
                        <td class = "uppertable" ><b>B :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >대부분의 나라들 만 나이 시스템을 사용해 사실, 만 나이 시스템에서 세는 것이 더 정확해.
                          게다가, 많은 의학 및 정부 서류들이 너의 만 나이를 적어달라고 요구해.</td>
                      </tr>

                    
                      </table>

        


      </div>
     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>When asked about your age, which age system do you prefer, Korean Age System or The Regular Age System? Why?</li>
          <li>Why should Korea continue using the traditional Korean Age System?</li>
          <li>What's your opinion about the abrogation of Korean Age System?</li>
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
