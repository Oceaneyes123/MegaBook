<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/young-friends-park_53876-46877.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Students Take A Gap Year?
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
      <td class = "lowertable" >For students that have been burned out from the pressures of high school and standardized testing, a gap year can be a chance to rest and reflect. Students are often unsure of what they want to pursue after high school, and the extra time to travel, work, or learn can be hugely beneficial. By taking this time, students often find themselves to be more well-rounded and have more experiences which turn out to be more attractive to admissions officers and employers.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Students, especially Korean males, only seem fit to join the army if they take a gap year. Gap years mean losing all the momentum of studying. They lose the structure and organization of school and could in fact end up wasting the year they take off along with scholarships and acceptances. Taking time off from studying can often derail a student from academics and can have them more lost and confused than they were before.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>burn out</b> 에너지를 소진하다
        </p>
        <p>
          <b>standardize</b> 표준화하다
        </p>
        <p>
          <b>reflect</b> 심사숙고하다
        </p>
        <p>
          <b>well-rounded</b> 다재다능한, 전인격을 갖춘
        </p>
        <p>
          <b>momentum</b> 추진력, 여세
        </p>
        <p>
          <b>acceptancem</b> 받아들임, 수락
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >고등학교의 압력과 표준화된 시험으로부터 에너지를 소진한 학생들에게 갭이어는 쉼을 갖고 반성을 하는 기회가 될 수 있습니다. 학생들은 주로 고등학교 이후 무엇을 추구하고 싶은지 확신하지 못하며 여행하고 일하고 혹은 배우는 추가적인 시간이 매우 유익할 수 있습니다. 이 시간을 가짐으로써 학생들은 주로 전인격적이 되고 입학사정관들이나 고용자들에게 더 매력적으로 보이는 경험들을 더 많이 가집니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >학생들, 특히 한국 남자들은, 갭이어를 가진다면 군대에 들어가기에 딱 맞게 보일 뿐입니다. 갭이어는 공부의 모든 추진력을 잃는 것을 의미합니다. 그들은 학교의 구조와 조직을 잃고 장학금과 입학허가와 함께 일 년을 낭비한 채로 끝날 수 있습니다. 학교로부터 벗어나는 것은 주로 학생들이 학업으로부터 탈선하게 만들며 전보다 더 방향을 잃고 혼란스럽게 할 수 있습니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you taken a gap year before? If not, have you considered taking one?</li>
          <li>Do you think it is a good idea for students to take a gap year? Why or why not?</li>
          <li>How does taking a gap year affect a student?</li>
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
