
<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/ghost-holding-wine-brick-wall_176420-16826.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Are Ghosts Real?
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
      <td class = "lowertable" >Ghosts exist, and there’s enough evidence out there that can prove they’re real. For instance, there are many photos with ghosts in them, and a lot of these pictures are pretty old. Some are more than 100 years old. Editing programs like Photoshop didn’t even exist back then. In addition, there are tons of ghost sightings. For example, a woman in Texas named April Ward temporarily closed down her restaurant after spotting a ghost in one of her surveillance videos. She said it freaked her out.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Ghosts aren’t real, and that’s a fact. Scientists and psychologists say that people think they see ghosts because of a phenomenon called “sensed presence.” It happens to people who feel stressed when they are isolated in an unfamiliar or unusual environment. Olaf Blanke, director of the Center for Neuroprosthetics, led a study that found that this stress tricks the brain into thinking that you are in the presence of a ghost. You might even think that an ancestor or a god is watching you.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>age-old</b> 아주 오래된
        </p>
        <p>
          <b>sighting</b> 목격
        </p>
        <p>
          <b>spot</b> 발견하다
        </p>
        <p>
          <b>surveillance</b> 감시
        </p>
        <p>
          <b>freak</b> 기겁을 하게 만들다
        </p>
        <p>
          <b>sense</b> 감지하다
        </p>
        <p>
          <b>presence</b> 있음, 존재(함)
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >귀신은 존재하고, 그들이 진짜라는 것을 증명할 충분한 증거가 있습니다. 예를 들어, 귀신이 들어있는 많은 사진들이 있고, 이 사진들 중 많은 것들이 꽤 오래되었습니다 어떤 것들은 100년 이상 된 것입니다 포토샵(Photoshop) 같은 편집 프로그램은 그 당시에는 존재하지도 않았습니다. 게다가, 귀신의 목격도 엄청 많습니다. 예를 들어, 텍사스(Texas)에 사는 에이프릴 워드(April Ward)라는 여성이 그녀의 감시 비디오에서 귀신을 발견한 후 그녀의 식당을 일시적으로 폐쇄했습니다. 그녀는 그것이 그녀를 겁먹게 만들었다고 말했습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >귀신은 실제가 아니며, 그것은 사실입니다. 과학자들과 심리학자들은 사람들이 "감지 된 존재"라고 불리는 현상 때문에 귀신을 보았다고 생각한다고 말합니다. 익숙하지 않은 환경에서 고립되었을 때 스트레스를 받는 사람들에게 일어난 일입니다. 신경 인성 센터의 책임자 인 올라프 브란케(Olaf Blanke)는 이 스트레스가 여러분이 귀신이 있다고 생각하도록 두뇌를 속이는 것을 발견한 연구를 주도했습니다 여러분은 심지어 조상이나 신이 여러분을 지켜보고 있다고 생각할 수도 있습니다 </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you believe that ghosts exist? Why or why not?</li>
          <li>Why do you think some people believe that ghosts are real while others don’t?</li>
          <li>Do you think people who claim that they can talk to ghosts are telling the truth? Why or why not?</li>
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
