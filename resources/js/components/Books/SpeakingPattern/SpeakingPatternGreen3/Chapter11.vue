<template>

<div :style = "{fontSize: fontSize + 'px'}">

<v-container fluid ma-0 pa-0>

  <v-layout column>
    <v-img
           src="https://image.freepik.com/free-photo/group-people-working-out-business-plan-office_1303-15773.jpg">

        <v-layout
        align-end
        fill-height
        pa-2
        black--text
      >
     <h1 class="upper-header-SPG3">~어때?
  </h1>
      </v-layout>
    </v-img>


          <h2 class="lower-header-SPG3">Today's topic</h2>

  <hr width="60%">
               <div style="padding : 10px; line-height: 200%;">

                 <h2>Pattern 51 |  </h2>
                  <br />
                  <h3>How about…?</h3>
                    <br />
                    <p>
                    How about…?은 상대방에게 제안을 할 때 많이 쓰이는 패턴이다. 뒤에 명사나 동명사 형태를 붙여주면 된다.
                    </p>
                    <br />

<h2 class = "border-SPG3">Dialogue
</h2>

<div style="padding-top : 10px; padding-bottom : 2px;">

          <br />
          <p style="line-height: 2;">
            A : We need to talk about the project.<br />
            B : <b>금요일에 만나는 건 어때?</b><br />
            A : No, it needs to be sooner, like today.<br />
            B : Okay.
          </p>
          <p style="line-height: 2;">
            A : 우린 프로젝트에 대해서 이야기해야 하.<br />
            B : <mark style="background-color: #a7d7c5; color: #d9e7cd;">How about meeting on Friday?</mark><br />
            A : 아니, 더 빨라야 할 것 같아. 오늘이라든지.<br />
            B : 좋아.
          </p>
          <br />


</div>

<h2  class = "border-SPG3">Pattern Practice
</h2>

<div style="padding-top : 10px; padding-bottom : 0px;">

        <br />

        <p>
          &rarr; 우리말을 보고 순식간에 영어로 말할 수 있을 때까지 반복하세요!
        </p>
        <br />

        <p>
          <b>401</b> 점심 먹을래? ( lunch ) <br />
        </p>
        <p>
          <b>402</b> 게임 한판 더 할까? ( another, game ) <br />
        </p>
        <p>
          <b>403</b> 금요일에 만날까? ( meet, Friday ) <br />
        </p>
        <p>
          <b>404</b> 파마하는 게 어때요? ( get, perm ) <br />
        </p>
        <p>
          <b>405</b> 영화 보러 가는 거 어때? ( go, movie ) <br />
        </p>
        <p>
          <b>406</b>  <br />
        </p>
        <p>
          <b>407</b>  <br />
        </p>
        <p>
          <b>408</b>  <br />
        </p>
        <v-container grid-list-md text-xs-left>
      <v-layout row wrap>


          <v-flex xs12>
          <v-card light color="#a7d7c5">
            <v-card-text class="px-10" style="color:#d9e7cd;">
              401 How about lunch?<br />
              402 How about another game?<br />
              403 How about meeting on Friday?<br />
              404 How about getting a perm?<br />
              405 How about going to the movie?<br />
              406 How about buying a new phone?<br />
              407 How about seeing a doctor?<br />
              408 How about you?<br />
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
  </v-container>

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


    }

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

<style lang="css">

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
