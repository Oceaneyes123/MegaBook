<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/female-volunteer-holding-clothes-donation-box_1170-1795.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-opinion1">Should we participate in volunteer work?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class="line-top-opinion1">
  </div>

  <h3  class = "lower-header-opinion1 white--text">Topic</h3>
  <div style = "line-height: 1.6;">
    <div style="padding : 16px;">   

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>A :</b></td>
      <td class = "lowertable" >I think we all need to take part in volunteering and social work.
      Nowadays, people are getting more selfish and living less grateful lives.
      I think spending some quality time away from a busy life will be helpful in gaining confidence and self-esteem.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>B :</b></td>
      <td class = "lowertable" >I totally agree with you.
      I have recently joined a volunteering organization in my neighborhood to help disabled people.
      It was a very rewarding experience and I started to feel grateful for the simple things in my life.</td>
    </tr>

    </table>

    </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>participate</b> in 참여하다
        </p>
        <p>
          <b>selfish</b> 제멋대로의
        </p>
        <p>
          <b>grateful</b> 감사하는
        </p>
        <p>
          <b>busy</b> 바쁜
        </p>
        <p>
          <b>gain</b> 얻다
        </p>
        <p>
          <b>self-esteem</b> 자존감
        </p>
        <p>
          <b>volunteer</b> 봉사
        </p>
        <p>
          <b>organization</b> 단체
        </p>
        <p>
          <b>rewarding</b> 보람이 있는
        </p>
        <p>
          <b>experience</b> 경험
        </p>
        <br />
        <p style="color: #56AAFF;">
          <b>take part in ~ ~에 참여하다.</b>
        </p>
        <p style="color: #56AAFF;">
          <b>disabled people 장애인</b>
        </p>

      </div>

      <div class = "line-opinion1">
      </div>
      <h3 class = "border-translate-opinion1 white--text">해석</h3>
      <div style="padding : 16px;">


                      <p class = "korean">
                        <b>
                        봉사활동에 참여해야 할까요?
                        </b>
                      </p>

                      <table class = "standard-table">

                       <tr>
                        <td class = "uppertable" ><b>A :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >우리 모두는 자원 봉사와 사회 사업에 참여 해야 한다고 생각해.
                          요즘 사람들은 점점 이기적으로 생활하고 덜 감사하는 삶을 살고 있어.
                          바쁜 삶에서 벗어나 좋은 시간을 보내면 자신감과 자부심을 얻는 데 도움이 될 거야.</td>
                      </tr>
                      <tr style="color:#1565C0;">
                        <td class = "uppertable" ><b>B :</b></td>
                        <td class = "lowertable" style = "word-break: keep-all" >나도 완전히 너에게 동의해.
                          나는 최근 장애인을 돕기 위해 이웃 에있는 자원 봉사 단체에 가입했어..
                          매우 보람 있는 경험 이었고 저는 제 인생의 단순한 것들에 감사하게 되었어.</td>
                      </tr>

                    
                      </table>


                   


      </div>

     <div class = "line-opinion1">
      </div>
      <h3 class = "border-opinion1 white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What springs to your mind when you hear the word ‘volunteer’?</li>
          <li>Have you ever volunteered to do something and then regretted volunteering? Why?</li>
          <li>Do you think we should all volunteer to do something good for others? In what ways?</li>
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

p{

  margin-top: 10px;
}

h3{
  padding-top: 7px;

}

body{

  font-size: 16px;
}

</style>
