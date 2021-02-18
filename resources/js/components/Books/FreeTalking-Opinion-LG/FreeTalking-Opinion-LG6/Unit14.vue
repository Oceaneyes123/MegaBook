
<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/serious-aged-professor-lecture-room-looking-camera_23-2148201090.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Collective Punishment In School Is Fair
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
      <td class = "lowertable" >What better way to police a class than have the students police themselves? Every class has a few students who talk too much, not do what they’re told, or misbehave like hitting other students. No matter how many times the teacher scolds or warns them, the troublemakers don’t seem to stop. If the rest of the class gets involved, however, the situation can change. A 2015 Chinese study found that collective punishment rather than collective reward better promotes social cooperation. Plus collective punishment can lead to a closer sense of community among classmates.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Collective punishment might have a good intention in mind, but the results are often bad. Why should the entire class suffer because of a few bad students? Doesn’t that go against the principle of individual responsibility? The system could also strain relations between the teacher and good students, who might resent being punished though they did nothing wrong. If anything, the logical conclusion can be that the class will grow to resent the bad students and the teacher instead of coming together overall. A few bad apples shouldn’t ruin things for the rest of the class.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>misbehave</b> 못된 짓을 하다, 비행을 저지르다
        </p>
        <p>
          <b>reward</b> 보상
        </p>
        <p>
          <b>police</b> 치안을 유지하다
        </p>
        <p>
          <b>troublemaker</b> 말썽꾼
        </p>
        <p>
          <b>collective</b> 집단의, 단체의
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >학생들이 스스로를 감시하는 교실을 유지하는 더 좋은 방법은 무엇일까요? 모든 교실은 너무 많이 말하거나 들은 것을 이행하지 않거나 다른 학생들을 때리는 것처럼 비행을 저지르는 몇몇 학생들이 있습니다. 선생님이 많이 야단을 치고 경고를 하더라도, 이 말썽꾼들은 멈출 것 같아 보이지 않습니다. 하지만, 만약 교실의 나머지 학생들이 휘말린다면, 상황을 변할 수 있습니다. 2015년 한 중국의 연구는 집단 체벌이 집단 보상보다 사회적 협력을 더 증진시킨다는 것을 발견했습니다. 게다가 집단 체벌은 반 친구들 사이에서 더 긴밀한 공동체 의식을 가져올 수 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >집단 체벌은 마음 속에 좋은 의도를 가질 수 있지만, 결과는 자주 나쁩니다. 왜 몇몇 나쁜 학생들 때문에 전체 학생이 처벌을 받아야 하나요? 이것은 각자의 책임의 원리에 위반하지 않습니까? 이 체계는 또한 자신들이 어떤 잘못된 일을 하지 않았음에도 처벌 받는 것에 분노하는 선생님과 좋은 학생들 사이의 관계를 경색시킬 수 있습니다. 만약 논리적인 결론을 내릴 수 있다면, 학생들을 전체적으로 단합시키는 대신 나쁜 학생들과 선생님에게 더 분노한다는 것입니다. 몇몇 암적인 존재들이 나머지 학생들을 위한 사과를 망치면 안 됩니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you been punished because of somebody else’s mistakes before?</li>
          <li>Do you think collective punishment is fair? Why or why not?</li>
          <li>What do you think is the best way to discipline a child</li>
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
