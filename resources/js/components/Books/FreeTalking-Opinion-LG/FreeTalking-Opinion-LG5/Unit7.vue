<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/mother-using-laptop-tablet-teaching-with-her-son-online-home-his-room_1328-3389.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Homeschooling Be Illegal?
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
      <td class = "lowertable" >I believe that we should stop allowing children to be homeschooled. Homeschooling often takes place at someone’s home, and the teachers are usually the student’s parents. Not all parents are experts in the subjects that they teach. Therefore, if a parent isn’t very good at math, then he or she will have a difficult time teaching it to their children. Furthermore, children who are homeschooled don’t have the convenience of school facilities. For example, most homes don’t have a gym or an art studio. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Homeschooling’s biggest advantage is that there is a lot more one-on-one attention. Many kids who go to school have trouble with certain classes, so they often fall behind because the teacher can’t provide them with the guidance they need. However, according to a study from Simon Fraser University, homeschooled kids can learn at their own pace. Parents can adjust the curriculum and make any necessary changes to a lesson plan to make sure that the child is receiving the best education possible. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>supervision</b> 관리, 감독
        </p>
        <p>
          <b>disadvantage</b> 불리한 점
        </p>
        <p>
          <b>expert</b> 전문가
        </p>
        <p>
          <b>convenience</b> 편의, 편리
        </p>
        <p>
          <b>provide</b> 제공하다
        </p>
        <p>
          <b>necessary</b> 필요한
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >저는 우리가 아이들이 홈스쿨링을 하도록 허락하는 것을 멈춰야 한다고 생각합니다. 홈스쿨링은 종종 누군가의 집에서 이뤄지고 선생님들은 대체로 그 학생의 부모들입니다. 모든 부모가 그들이 가르치는 과목의 전문가들은 아닙니다. 그래서 만약 한 부모가 수학을 잘하지 못하면 그 또는 그녀는 그것을 아이들에게 가르치기 힘들 것입니다. 또한 홈스쿨링을 하는 아이들은 학교 시설의 편의성을 가지지 못합니다. 예를 들어 대부분의 가정은 체육관 또는 미술실을 가지고 있지 않습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >홈스쿨링의 가장 큰 이점은 일대일 집중이 많다는 것입니다. 학교에 다니는 많은 아이들이 어떤 수업에 어려움을 갖고 있습니다, 그래서 그들은 선생님이 그들이 필요한 가이드를 제공하지 못해서 종종 뒤쳐집니다. 그러나 사이먼 프래이져 대학의 한 연구에 따르면 홈스쿨링을 하는 아이들은 그들의 고유한 속도에 따라 배울 수 있습니다. 학부모는 교과 과정을 조정하고 가능한 한 최상의 교육을 받을 수 있도록 수업 계획을 변경할 수 있습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are your thoughts on homeschooling?</li>
          <li>What do you believe are its advantages and disadvantages?</li>
          <li>Would you let your kids be homeschooled? Why or why not?</li>
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
