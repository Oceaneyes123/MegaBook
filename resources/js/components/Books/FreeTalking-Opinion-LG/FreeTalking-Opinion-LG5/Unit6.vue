<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/pile-3d-popular-social-media-logos_1379-881.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Social Media Good For Our Society?
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
      <td class = "lowertable" >Social media is excellent! Social networking sites actually help students do better at school. Almost 60 percent of students with internet access say that they use social media to talk about education, and around 50 percent use it to talk about homework and other school projects. Interestingly, a middle school in Oregon introduced a social media program and students’ grades went up by 50 percent, absences went down by 33 percent, and 20 percent of the students completed their extra-credit assignments. How amazing is that? </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Social media has many disadvantages, but one of its biggest problems is that it spreads false information. More than half of all Twitter users who visit it for news say that they have come across something they later discovered was false. To make it worse, it has been discovered that false information spreads six times faster than actual news on Twitter. In addition, three months before the 2016 U.S. presidential election, inaccurate information about the two candidates was shared 37.6 million times on Facebook.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>support</b> 지지하다
        </p>
        <p>
          <b>benefit</b> 장점
        </p>
        <p>
          <b>distracting</b> 마음을 산란케 하는
        </p>
        <p>
          <b>absence</b> 결석
        </p>
        <p>
          <b>spread</b> 퍼뜨리다
        </p>
        <p>
          <b>false</b> 거짓된
        </p>
        <p>
          <b>inaccurate</b> 부정확한
        </p>
        <p>
          <b>candidate</b> 후보
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >소셜 미디어는 훌륭합니다! 소셜 네트워킹 사이드들은 사실 학생들이 학교에서 더 잘할 수 있도록 돕습니다. 인터넷 접속이 되는 60퍼센트 가량의 학생들이 교육에 대해 이야기하기 위해 소셜 미디어를 사용하고, 50퍼센트 정도가 숙제와 다른 학교 프로젝트에 대해 이야기하기 위해 그것을 사용한다고 말합니다.흥미롭게도 오리건 주의 한 중학교는 한 소셜 미디어 프로그램을 소개하고 학생들의 성적이 50퍼센트 올랐고, 결석이 33퍼센트 줄었으며, 20퍼센트의 학생들이 그들의 가산점 과제를 완성했습니다. 그것은 얼마나 놀랍습니까? </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >만약 여러분이 더 오래 살고 싶다면, 커피를 마셔야 합니다. 뉴 잉글랜드 의학 저널 (New England Journal of Medicine)의 한 연구에 따르면 하루 6 잔 이상의 커피를 마시는 사람들은 그렇지 않은 사람들에 비해 사망 위험이 10-15 % 낮습니다 또한 커피는 심장 건강에 좋습니다. 미국 심장 협회(American Heart Association )저널에 실린 네덜란드(Dutch) 연구 논문에 따르면 커피를 마시는 사람은 심장 질환 위험이 20 % 낮습니다. 소셜 미디어는 많은 단점을 가지고 있습니다, 그러나 그것의 가장 큰 문제들 중 하나는 거짓 정보를 퍼트린다는 것입니다. 뉴스를 보기 위해 방문하는 모든 트위터 사용자들 중 절반 이상이 나중에 거짓이라고 밝혀진 어떤 정보를 접했다고 말합니다. 더 나쁜 것은, 트위터 상에서 실제 뉴스보다 잘못된 정보가 6배나 빠르게 퍼진다는 것이 밝혀졌습니다. 더욱이 2016 미국 대선 3개월 전에 두 후보에 대한 정확하지 않은 정보가 페이스북 상에서 3,760만 번 공유되었습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Are you fond of using social networking sites? If yes, what sites do you frequent?</li>
          <li>Do you find social media helpful? If yes, how so? If not, why?</li>
          <li>How do you think social media affects society?</li>
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
