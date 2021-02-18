<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/london-motorcycle-police_1426-1642.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Always Respect The Police?
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
      <td class = "lowertable" >The police of the world serve a purpose in preventing and eradicating crime. When criminals break the law and hurt others, the police is the best way to ensure safety. When you look at countries with high GDP rates and safety levels, there is always a solid police system involved. Police are educated in the best ways to protect and serve civilians. They must go through tests and receive training in ethics, justice, and preserving peace. There are multiple ways for police to protect and serve. They are given permission to calmly suppress violent situations. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Sometimes police do not do things for our best interest. In America alone, the #BlackLivesMatter movement put law enforcement in a dark light. While their jobs are to protect and serve, in many cases police have been known to be biased. This can manifest itself in punishments that may be too extreme. In many cases, police in America have often followed a ‘warrior cop’ mentality with the rate of gun violence and shooting of innocent civilians rising every year. Just because they are in a uniform and meant to protect you does not mean they will always do so. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>brutality</b> 잔인성
        </p>
        <p>
          <b>terrorize</b> 공포에 떨게 하다
        </p>
        <p>
          <b>eradicate</b> 근절하다, 뿌리뽑다
        </p>
        <p>
          <b>solid</b> 기반이 탄탄한
        </p>
        <p>
          <b>civilian</b> 민간인
        </p>
        <p>
          <b>permission</b> 허가, 허락
        </p>
        <p>
          <b>calmly</b> 침착하게, 태연하게
        </p>
        <p>
          <b>suppress</b> 진압하다
        </p>
        <p>
          <b>manifest</b> (특질을 분명히) 나타내다
        </p> 
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >세계의 경찰은 범죄를 예방하고 근절하는 목적을 수행합니다. 범죄자들이 법을 어기고 다른 사람들에게 상처를 입히면, 경찰이 안전을 보장하는 최고의 방법입니다. GDP 비율과 안전 수준이 높은 나라들을 보면, 항상 견고한 경찰 체계가 있습니다. 경찰은 시민들을 보호하고 섬기는 최고의 방법들을 교육 받습니다. 그들은 시험을 보고, 윤리, 법 그리고 평화 유지 훈련을 받아야 합니다. 경찰이 보호하고 섬기는 데에는 많은 방법이 있습니다. 그들은 폭력적인 상황을 조용히 억압하는 허가를 받습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >때때로 경찰은 우리의 최고의 이익을 위해 일을 하지 않습니다. 미국만 보더라도 #BlackLivesMatter운동은 사법 집행부를 어둡게 바라봅니다. 그들의 직업이 보호하고 섬기는 것인 반면, 많은 경우 경찰은 편향된 것으로 알려져 왔습니다. 이것은 매우 극단적일 수 있는 처벌에서 나타날 수 있습니다. 많은 경우, 미국의 경찰은 총 사용과 매년 증가하는 선량한 시민들을 향한 발포 비율이 증가하면서 ‘전사 경찰’ 정신을 따릅니다. 그들이 제복을 입고 당신을 보호하도록 의도되었다고 해서 그것이 항상 그런 것은 아닙니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>How would you describe a police officer?</li>
          <li>How do police officers help its country's citizens?</li>
          <li>Do you know about the #BlackLivesMatter? What are your thoughts about it?</li>
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
