<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/classmates-working-together_1098-2588.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Korea Should Abolish Same-Sex Schools
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
      <td class = "lowertable" >Korea’s practice of having single-sex schools needs to stop. Attending an all-boys school distorts reality because women comprise half of the population, so boys and girls need to get used to being together in school. Plus the stereotype that boys are X and girls are Y is often flawed; certain boys might exhibit traits usually associated with girls like shyness and sensitivity or certain girls can exhibit what could be considered machismo. One study also found that having girls in the classroom helped to raise the overall achievement of the class.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Single-sex schools are popular in Korea not because the country is sexist, but because such a system works. A University of Pennsylvania study conducted in Korea assigned students to single-sex and coed schools. The students in singlesex classrooms were found to be more likely to attend universities and score higher on tests. Several schools in Korea have gone back to being single sex instead of coed because of student choice. And in Korea, where appearance is important, looks seem less important at a single-sex school than it might at a coed one.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>coed (co-education)</b> 학교나 교육제도가 남녀공학의
        </p>
        <p>
          <b>inherent</b> 내제하는
        </p>
        <p>
          <b>comprise</b> ~으로 구성되다
        </p>
        <p>
          <b>shyness</b> 수줍음
        </p>
        <p>
          <b>sensitivity</b> 상처를 잘 받는 예민함, 민감함
        </p>
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >동성 학교를 만드는 한국의 제도는 멈출 필요가 있습니다. 여성이 인구의 반을 차지하기에 남학교를 다니는 것은 현실을 왜곡시키고 남학생과 여학생은 학교에서 같이 존재하는 것에 익숙해질 필요가 있습니다. 게다가 남학생들이 X이고 여학생들은 Y라는 고정관념은 자주 결함이 있는데, 몇몇 남학생들은 수줍음과 민감함과 같은 여학생들에 보통 관련되는 특성들을 보이기도 하며 몇몇 여학생들은 남자다움으로 간주될 수 있는 것들을 보일 수 있습니다. 한 연구는 또한 교실에 여학생을 갖는 것이 학급의 전체적인 성취를 올려주는 데 도움을 준다고 발견하였습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >동성을 다니는 학교는 나라가 성차별주의이기 때문에 인기가 있는 것이 아니라, 그러한 시스템이 효과가 있기에 존재하는 것입니다. 한국에서 시행된 펜실베니아 대학의 한 연구는 학생들을 동성이 다니는 학교와 남녀공학에 배치하였습니다. 동성만이 있는 교실의 학생들은 대학에 진학할 확률이 높고 시험에서 더 높은 점수를 얻는 가능성이 더 큰 것으로 발견되었습니다. 한국의 몇몇 학교들은 학생들의 선택으로 인해 남녀 공학 대신 동성 학교로 다시 돌아갔습니다. 그리고 외모가 중요시되는 한국에서, 동성이 다니는 학교에서는 남녀 공학보다 외모가 덜 중요하게 보입니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>WWhat do you think of same-sex schools?</li>
          <li>Do you agree that same-sex schools should be abolished? Why or why not?</li>
          <li>Would you want your child to go to a same-sex school? Why or why not?</li>
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
