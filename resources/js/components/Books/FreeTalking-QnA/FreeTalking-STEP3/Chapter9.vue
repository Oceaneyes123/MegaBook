<template>

<div :style = "{fontSize: fontSize + 'px'}">

<v-container fluid ma-0 pa-0>

  <v-layout column>
    <v-img
           src="https://marketplace.canva.com/fsK3Q/MADyQ7fsK3Q/1/s2/canva-people-playing-poker-MADyQ7fsK3Q.jpg" class="cover-photo-FTQNA3" >

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
      >
        <h1 class="upper-header-FTQNA3">Gambling</h1>
      </v-layout>
    </v-img>


          <h3 class="border-FTQNA3">Q &amp; A</h3>
               <div style="padding : 16px;">

   <ol style="margin: 12px;">
     <li class="mb-2">
        Why do people gamble? Give five reasons.
     </li>
     <br />
     <li class="mb-2">
        When did you gamble last?
        <ul>
        <li class="mt-2"> What game did you play? Where?</li>
        <li> Did you win or lose the last time you gambled? </li>
        <li> What did you win or lose?</li>
        </ul>
     </li>
     <br />
     <li class="mb-2">
          Have you ever gambled and lost a lot of money?
     </li>
     <br />
     <li class="mb-2">
         Is gambling legal in your country?
        <ul>
        <li class="mt-2"> What kind, if any?</li>
        <li> If not, why isn't it legal?</li>
        <li> Do you think that gambling should be legal or illegal? Why?</li>
        </ul>
     </li>
   </ol>



</div>

<h3 class="border-FTQNA3">Translation</h3>
               <div style="padding : 16px;">

   <ol style="margin: 12px;">
     <li class="mb-2">
        사람들은 왜 도박을 할까요? 다섯 가지 이유를 제시하세요.
     </li>
     <br />
     <li class="mb-2">
        도박은 언제 마지막으로 했어요?
        <ul>
        <li class="mt-2">무슨 게임을 했어요? 어디서요?</li>
        <li>지난번 도박에서 이겼나요? 아니면 졌나요?</li>
        <li>당신은 무엇을 이기고 무엇을 잃었나요?</li>
        </ul>
     </li>
     <br />
     <li class="mb-2">
          당신은 도박을 해서 많은 돈을 잃은 적이 있나요?
     </li>
     <br />
     <li class="mb-2">
         당신 나라에서는 도박이 합법적인가요?
        <ul>
        <li class="mt-2">만약 있다면 어떤 종류인가요?</li>
        <li>만약 그렇지 않다면, 왜 그것이 합법적이지 않나요?</li>
        <li>당신은 도박이 합법이어야 한다고 생각합니까, 아니면 불법이어야 한다고 생각합니까? 왜요?</li>
        </ul>
     </li>
   </ol>



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

ul {
  list-style-type: none;
}

ul > li:before {
  content: "–"; /* en dash */
  position: absolute;
  margin-left: -1.1em;
}

</style>
