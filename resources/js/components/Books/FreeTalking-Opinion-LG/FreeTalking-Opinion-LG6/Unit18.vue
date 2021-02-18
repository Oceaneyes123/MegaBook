<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/3d-surreal-mars-style-landscape_1048-9878.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Flying To Mars A Waste Of Time And Money?
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
      <td class = "lowertable" >We should stop trying to fly humans to Mars. It’s a waste of time and money. Space architect Brent Sherwood said the benefit of manned missions to Mars doesn’t justify the huge costs. One of his main arguments is that robots can do more advanced research in space than humans can. Also, robotic missions are much cheaper and puts no human lives at risk.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >We shouldn’t stop trying to fly humans to Mars. Many places on Earth would have been left undiscovered if discoverers never explored new lands. Their curiosity and determination to learn more about the world led to new civilizations. It will be a great achievement for humans to explore planets other than Earth. It costs a lot of time and money to explore Mars but it’s worth it to learn more about another planet. We can’t give up now!</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>architect</b> 건축가
        </p>
        <p>
          <b>benefit</b> 혜택
        </p>
        <p>
          <b>curiosity</b> 호기심
        </p>
        <p>
          <b>civilization</b> 문명
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >우리는 인간을 화성에 보내는 것을 그만두어야 합니다. 그것은 시간과 돈 낭비입니다. 우주선 설계자 브랜드 셜우드는 유인화성탐사의 이득이 거대한 비용을 정당화하지 않는다고 말했습니다. 주요한 주장들 중 하나는 로봇이 인간보다 우주에서 더 진보된 연구를 할 수 있다는 것입니다. 또한 로봇탐사는 더 저렴하며 인간 생명에 대해 위험을 감수하지 않습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >우리는 인간을 화성에 보내기를 중단하면 안 됩니다. 만약 탐사자들이 새로운 땅을 탐험하지 않았다면, 지구의 많은 지역들은 발견되지 않은 채로 남았을 것입니다. 그들의 호기심과 세계에 대해 더 알고자 하는 결심은 새로운 문명을 낳았습니다. 인간이 지구 외에 다른 행성을 탐험하는 것은 위대한 성취가 될 것입니다. 화성을 탐험하는 데 많은 시간과 돈이 들지만 다른 행성에 대해 더 배워가는 것은 가치가 있습니다. 우리는 지금 포기하면 안 됩니다!</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are your thoughts on space explorations?</li>
          <li>Do you agree that flying to Mars is a waste of time and money? Why or why not?</li>
          <li>Given a chance, would you also fly to Mars? Why or why not?</li>
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
