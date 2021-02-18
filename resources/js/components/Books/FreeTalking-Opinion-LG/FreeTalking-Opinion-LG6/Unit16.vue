<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/close-up-marble-table-with-technological-equipment_1156-41.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Educational Technology Useful in the Classroom?
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
      <td class = "lowertable" >Technology has improved daily life for humans, and promises to do so again in the classroom. Educational technology allows students to hear lectures online from anywhere in the world, use interactive programs that promote learning, and boost independent learning. It also makes students more tech savvy, a skill that will prove crucial for their future. The proliferation of e-textbooks and e-classes will also lead to lower costs for textbooks and tuition. And such technology could make learning more fun as many students find the traditional lecture and textbook method boring. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Educational technology’s disadvantages outweigh the advantages. At a time of rising youth addiction to digital screens, using tablet PCs or mobile phone apps for studying could worsen the digital addiction problem and make students lazier. Technology seems more for entertainment, not education. So students are more likely to use a book to learn but a tablet to play games or use social media. And studies have shown that those who take online courses have a higher chance of failing and dropping out, and are less likely to benefit from them.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>interactive</b> 상호 작용의
        </p>
        <p>
          <b>boost</b> 증가시키다
        </p>
        <p>
          <b>tech-savvy</b> 테크놀로지, 즉 최신기술에 능통한
        </p>
        <p>
          <b>proliferation</b> 확산
        </p>
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >기술은 인간의 일상적인 삶을 개선시켜 왔으며 교실에서도 그렇게 할 수 있다고 약속합니다. 교육 기술은 학생들이 세계 어디서나 온라인으로 강의를 듣고, 학습을 촉진하는 상호적인 프로그램을 사용하고 독립적인 배움을 증진시키도록 해 줍니다. 그것은 또한 학생들을 더욱 기술에 능통하게 만드는데, 이것은 그들의 미래에서 매우 중요해질 능력입니다. 전자 교과서와 온라인 수업의 증식은 또한 교과서와 수업을 위한 비용을 낮출 것입니다. 이러한 기술은 많은 학생들이 전통적인 강의와 교과서를 지루하게 느낌에 따라 배움을 더 재미있게 해줄 것입니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >교육 기술의 단점이 장점보다 큽니다. 젊은이들이 디지털 화면에 대해 점점 중독되고 있는 이와 같은 시기에, 공부를 위해 테블릿 PC와 핸드폰을 사용하는 것은 디지털 중독의 문제를 악화시키고 학생들을 더 게으르게 만들 것입니다. 테크놀로지는 교육이 아니라 오락을 위한 것처럼 보입니다. 따라서 학생들은 배우기 위해선 책을 사용하고 게임을 하거나 소셜 미디어를 하기 위해선 테블릿을 사용할 가능성이 높습니다. 또한 연구는 온라인 수업을 듣는 사람들이 낙제와 중퇴를 당하는 더 높은 가능성을 가지고 있어 기술들로부터 이점을 얻기에는 가능성이 낮습니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are your thoughts on educational technology?</li>
          <li>What are the benefits of educational technology in the classroom?</li>
          <li>Do you think educational technology does more harm than good? Why or why not?</li>
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
