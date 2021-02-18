<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/abstract-background-with-planets-space_23-2148235955.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Are Aliens Real?
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
      <td class = "lowertable" >Many years ago, people thought there was something beyond the sky. But now,
      we can easily see actual photos of space.
      We don't have much evidence that aliens exist, but it's too early to say that there are no aliens.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>B :</b></td>
      <td class = "lowertable" >Some researchers say they have evidence that aliens are real, but NASA and many scientists are not convinced.
      News about aliens and spaceships don't last very long.
      This means that aliens are imaginary creatures like unicorns.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>think</b> 생각하다
        </p>
        <p>
          <b>beyond</b> ~저편에
        </p>
        <p>
          <b>actual</b> 실제의
        </p>
        <p>
          <b>evidence</b> 증거
        </p>
        <p>
          <b>exist</b> 존재하다
        </p>
        <p>
          <b>early</b> 이른
        </p>
        <p>
          <b>researcher</b> 연구원
        </p>
        <p>
          <b>convinced</b> 확신하는
        </p>
        <p>
          <b>imaginary</b> 상상에만 존재하는
        </p>
        <p>
          <b>creature</b> 생물
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">


                      <p class = "korean">
                        <b>
                        외계인은 진짜인가?
                        </b>
                      </p>

                      <table class = "standard-table">

                       <tr>
                        <td class = "uppertable" ><b>A :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >오래 전에, 사람들은 하늘 너머에 뭔가가 있다고 생각했습니다.
                        하지만 이제는 실제 공간 사진을 쉽게 볼 수 있습니다.
                        우리는 외계인이 존재한다는 증거를 많이 가지고 있지 않지만,
                        외계인이 없다고 말하기는 너무 이릅니다.</td>
                      </tr>
                      <tr style="color:#1565C0;">
                        <td class = "uppertable" ><b>B :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >몇몇 연구원들은 외계인이 존재한다는 증거를 가지고 있다고 말하지만,
                        나사와 많은 과학자들은 확신하지 못합니다. 외계인과 우주선에 대한 소식은 그리 오래 가지 않습니다.
                        이것은 외계인이 유니콘과 같은 상상의 생물이라는 것을 의미합니다.</td>
                      </tr>

                    
                      </table>


      </div>
     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you think aliens exist? Why or Why not?</li>
          <li>How would you feel if aliens visit the earth? Why?</li>
          <li>What do you think aliens might look like?</li>
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
