<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/cropped-view-young-people-using-smartphones_74855-5037.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Ban Students From Using Social Media

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
      <td class = "lowertable" >A 2013 research paper said teenagers consider school and family time “pauses” in their online social existences. In other words, they deem their cyberspace lives more important than their real lives. Thus potential pitfalls in social media abound. Cyberbullying is a problem best avoided in a country where bullying is a chronic issue. Students are also ill-equipped to handle the rigors of cyberspace like harsh criticism, trolls, and fake news. Just as the consumption of cigarettes, adult material, and alcohol has a minimum age, so should social media.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Social media has both pluses and minuses, but let students learn for themselves. Facebook has allowed many youths to connect with people worldwide and gain experiences they could never have if social media didn’t exist. One study also found that students tend to keep in touch with friends more through social media, which is good for boosting friendships. Moreover, an online community for subjects can help students in certain subjects through group chats or location of supplementary materials. So social media isn’t the problem, it’s the incorrect use of it.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>side effect</b> 부작용
        </p>
        <p>
          <b>deem</b> ~로 여기다
        </p>
        <p>
          <b>pitfall</b> 눈에 잘 안 띄는 위험
        </p>
        <p>
          <b>abound</b> 아주 많다
        </p>
        <p>
          <b>supplementary</b> 보충의
        </p>
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >2013년에 발표된 한 연구에는 청소년이 학교와 가족과의 시간을 그들의 온라인 사회적 존재에 있어 “정지”로 간주한다고 말하였습니다. 다른 말로, 그들은 사이버공간을 그들의 실세계보다 더 중요하게 생각합니다. 따라서 잠재적인 위험이 소셜미디어에 넘쳐나고 있습니다. 사이버왕따는 왕따가 고질적인 문제로 있어왔던 나라에 있어 반드시 피해져야 하는 문제입니다. 학생들은 또한 거친 비난이나, 트롤 그리고 가짜뉴스와 같은 사이버공간의 가혹한 행위들을 잘 다루지 못합니다. 담배, 성인용 자료 그리고 술 소비에 최저연령이 있듯이 소셜미디어도 그래야 합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >소셜미디어는 장점과 단점 둘 다 있지만 학생들이 그들 자신을 위해 배우게 해줍니다. 페이스북은 많은 젊은이들이 전 세계에 있는 사람들과 연결시켜주고 소셜미디어가 존재하지 않았다면 가질 수 없었던 경험들을 갖게 해줍니다. 한 연구는 또한 학생들이 소셜 미디어를 통해 더 많은 친구들과 접촉을 하고 있는 것을 발견하였는데 이것은 우정을 증진시키는 데 유익하다. 더욱이 다양한 주제에 대한 온라인 공동체는 학생들이 그러한 주제들에 대해 그룹 채팅이나 보충자료를 찾음으로써 배우도록 도와줍니다. 따라서 소셜미디어가 문제가 아니며 문제는 그것의 부적절한 사용입니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you think social media is important? Why or why not?</li>
          <li>What are the pros and cons of social media for students?</li>
          <li>What netiquette would you advise students to always keep in mind?</li>
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
