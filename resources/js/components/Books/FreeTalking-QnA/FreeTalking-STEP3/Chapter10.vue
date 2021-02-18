<template>

<div :style = "{fontSize: fontSize + 'px'}">

<v-container fluid ma-0 pa-0>

  <v-layout column>
    <v-img
           src="https://image.freepik.com/free-photo/calculator-with-coins-table_23-2147931207.jpg" class="cover-photo-FTQNA3" >

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
      >
        <h1 class="upper-header-FTQNA3">Government Spending</h1>
      </v-layout>
    </v-img>


          <h3 class="border-FTQNA3">Q &amp; A</h3>
               <div style="padding : 16px;">

   <ol style="margin: 12px;">
     <li class="mb-2">
        What are some programs the government of your country spends money on?
     </li>
     <br />
     <li class="mb-2">
        If you were the president or leader of your country, what would you change in your country's budget?
     </li>
     <br />
     <li class="mb-2">
        If you had the power to cut government spending, what programs would you eliminate? Why?
     </li>
     <br />
     <li class="mb-2">
        Do you think your government spends its money wisely? Why or why not?
     </li>
   </ol>



</div>

<h3 class="border-FTQNA3">Translation</h3>
       <div style="padding : 16px;">

   <ol style="margin: 12px;">
     <li class="mb-2">
        당신 나라 정부가 돈을 쓰는 프로그램은 무엇입니까?
     </li>
     <br />
     <li class="mb-2">
        만약 당신이 당신의 나라의 대통령이나 지도자라면, 당신의 나라 예산에서 무엇을 바꾸겠습니까?
     </li>
     <br />
     <li class="mb-2">
        만약 여러분이 정부 지출을 줄일 수 있는 힘이 있다면, 어떤 프로그램을 없앨 건가요? 왜요?
     </li>
     <br />
     <li class="mb-2">
        여러분은 정부가 돈을 현명하게 쓴다고 생각하나요? 왜 그렇게 생각하나요, 아니라면 왜 아니라고 생각하나요?
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
