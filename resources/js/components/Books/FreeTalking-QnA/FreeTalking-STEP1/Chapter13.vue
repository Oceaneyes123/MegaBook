<template>

<div :style = "{fontSize: fontSize + 'px'}">

<v-container fluid ma-0 pa-0>

  <v-layout column>
    <v-img
           src="https://marketplace.canva.com/i1AjM/MAD3hfi1AjM/1/s2/canva-man-in-blue-sweater-having-a-sweet-conversation-MAD3hfi1AjM.jpg" class="cover-photo-FTQNA1">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
      >
        <h1 class="upper-header-FTQNA1">Communication</h1>
      </v-layout>
    </v-img>


          <h3 class="border-FTQNA1">Q &amp; A</h3>
               <div style="padding : 16px;">

   <ol style="margin: 12px;">
     <li>
       Talk about the differences between making a phone call and writing a letter.<br />
       <br />
     </li>
     <li>
       Do you think it's okay to use company phones for personal business?<br />
       <br />
     </li>
     <li>
       How many letters did you write to your wife or husband before you were married?<br />
       <br />
     </li>
     <li>
       What kind of information do you get from the internet?<br />
       <br />
     </li>
     <li>
       Talk about common courtesy in using mobile phones in public areas.
     </li>
   </ol>

</div>

<h3 class="border-FTQNA1">Translation</h3>
<div style="padding : 16px;">

  <ol style="margin: 12px;">
     <li class="mb-2">
       전화 통화와 편지 쓰기의 차이점에 대해 이야기해보세요.
     </li>
     <br />
     <li class="mb-2">
       개인 업무용으로 회사 전화를 사용해도 괜찮을까요?
     </li>
     <br />
     <li class="mb-2">
       결혼하기 전에 아내나 남편에게 몇 통의 편지를 썼습니까?
     </li>
     <br />
     <li class="mb-2">
       당신은 인터넷에서 어떤 종류의 정보를 얻습니까?
   </li>
   <br />
   <li class="mb-2">
       공공장소에서 휴대폰을 사용하는 것에 대한 일반적인 예의에 대해 이야기해보세요.
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
