
<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/old-vintage-camera-old-books-wooden-background-old-vintage-holiday-concept_1220-1115.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should we go back to film photography?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class = "line-top-lg">
  </div>
  <h3  class = "lower-header-lg white--text">Topic</h3>

  <div style = "padding : 16px; line-height: 1.6;">

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>David :</b></td>
      <td class = "lowertable" >Vintage is back! Wherever you look, you can see traces of history making a comeback into mainstream society. From vintage clothing and accessories to vinyl records, old classics are new again. While digital photography has changed the world, it hasn’t necessarily for the better. Audiophiles listen to music on vinyl records because the sound is truer than a digital MP3. In the same way, photo purists believe there is a quality to film photography that digital photos cannot match!</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Unfortunately, film photography is dead. There may be something cool about using something from the past, but digital photography is here to stay. Whether you are using a DSLR, a mirrorless camera, or your smartphone, digital images have become a way of life in our Snapchat, Instagram, and Facebook world. InfoTrends estimates over 1 trillion photos were snapped in 2015 alone. Realistically, we’re not going to go back to the days of rewinding film, using smelly chemicals, and paying for film processing.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>purist</b> 순수주의자
        </p>
        <p>
          <b>vintage</b> 고전적인, 유서 깊은
        </p>
        <p>
          <b>mainstream</b> 주류
        </p>
        <p>
          <b>audiophile</b> 오디오(음향) 애호가
        </p>
        <p>
          <b>match</b> 맞먹다, 필적하다
        </p>
        <p>
          <b>estimate</b> 추정, 추산하다
        </p>
        <p>
          <b>rewind</b> 되감다
        </p>
        <p>
          <b>process</b> 처리하다
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >고전이 돌아왔습니다! 어디를 보더라도 여러분은 역사의 흔적들이 주류 사회로 돌아오고 있는 흔적들을 볼 수 있습니다. 옛 옷과 장신구들에서부터 레코드판들까지 오래된 고전들이 다시 쓰이고 있습니다. 디지털 사진 기술이 세상을 바꾸긴 했지만 그것은 확연하게 발전하지는 않았습니다. 음향 애호가들은 디지털 MP3 보다 더욱 진실된 소리를 들려주기 때문에 레코드판들로 음악을 듣습니다. 이런 의미에서 사진 애호가들은 필름 사진술에 디지털 사진들이 대적할 수 없는 품질이 있다고 믿습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >안타깝지만, 필름 사진은 끝났습니다. 과거의 유물을 사용하는 것이 멋져 보일 수는 있겠지만, 디지털 사진술은 지속될 것입니다. 여러분이 DSLR, 미러리스 카메라, 또는 여러분의 스마트폰을 사용하던지, 디지털 사진들은 스냅챗, 인스타그램 그리고 페이스북의 세계에서 우리 삶의 방식이 되었습니다. 인포트렌즈는 2015년에만 해도 1조 개가 넘는 사진들이 찍혔다고 말했습니다. 현실적으로, 우리는 필름을 감고, 냄새나는 화학물질들을 쓰며, 사진 현상을 위해 돈을 쓰는 날들로 되돌아가지 않을 것입니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like taking pictures? Why or why not?</li>
          <li>Have you ever tried taking pictures using a film camera?</li>
          <li>Do you think film photography is better than digital photography? Why or why not?</li>
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

</style>
