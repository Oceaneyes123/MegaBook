<template>

<div :style = "{fontSize: fontSize + 'px'}">

<v-container fluid ma-0 pa-0>

  <v-layout column>
    <v-img
           src="https://image.freepik.com/free-photo/group-three-young-multi-ethnic-successful-business-people-sitting-coworking-space-talking-about-new-project-competitor-team-making-plans-bypass-their-project_176420-8311.jpg">

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

                 <h2>Pattern 52 |  </h2>
                  <br />
                  <h3>What about…?</h3>
                    <br />
                    <p>
                    이 패턴은 How about…? 과 똑같이 상대방에게 제안을 할 때 아주 유용하다. 길게 설명할 필요 없이 What about 뒤에 하고 싶은 것만 붙이면 간단하면서도 멋진 제안이 된다.
                    </p>
                    <br />

<h2 class = "border-SPG3">Dialogue
</h2>

<div style="padding-top : 10px; padding-bottom : 2px;">

          <br />
          <p style="line-height: 2;">
            A : So when can we get together?<br />
            B : <b>내일 어때?</b><br />
            A : I can’t. I’m completely booked. How about Thursday?<br />
            B : That’s fine with me.
          </p>
          <p style="line-height: 2;">
            A : 그래서 우리 언제 만날 수 있는 거야?<br />
            B : <mark style="background-color: #a7d7c5; color: #d9e7cd;">What about tomorrow?</mark><br />.
            A : 안 돼. 난 꼼짝 못해. 목요일은 어떠니?<br />
            B : 난 괜찮아.<br />

            * Be booked 약속이 있다.
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
          <b>409</b> 내일은 어때? ( tomorrow ) <br />
        </p>
        <p>
          <b>410</b> 스미스 가족을 초대하는 게 어때요? ( invite ) <br />
        </p>
        <p>
          <b>411</b> 저녁에 좋은 와인 한 병 곁들이는 건 어떨까? ( a bottle of wine, dinner ) <br />
        </p>
        <p>
          <b>412</b> 네 배낭에 이걸 가져갈래? ( carry, backpack )  <br />
        </p>
        <p>
          <b>413</b> 이거는 어때? ( this one ) <br />
        </p>
        <p>
          <b>414</b>  <br />
        </p>
        <p>
          <b>415</b>  <br />
        </p>
        <p>
          <b>416</b>  <br />
        </p>
        <v-container grid-list-md text-xs-left>
      <v-layout row wrap>


          <v-flex xs12>
          <v-card light color="#a7d7c5">
            <v-card-text class="px-10" style="color:#d9e7cd;">
              409 What about tomorrow?<br />
              410 What about inviting the Smith family?<br />
              411 What about a nice bottle of wine with dinner?<br />
              412 What about carrying this in your backpack?<br />
              413 What about this one?<br />
              414 What about your dreams?<br />
              415 What about the other school you were considering?<br />
              416 What about spaghetti and meatballs?<br />
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
