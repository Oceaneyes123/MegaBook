<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/brunette-woman-getting-her-hair-cut_23-2148108792.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" class="upper-header-lg">[08/20] Short Hair Versus Long Hair
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class="line-top-lg">
  </div>

  <h3  class = "lower-header-lg white--text">Topic</h3>
  <div style = "padding : 16px; line-height: 1.6;">

    <table style = "border-collapse: collapse;">

    <tr>
      <td class = "uppertable" ><b>Jane :</b></td>
      <td class = "lowertable" >Long hair is better than short hair because there are more styling options. There’s not much you can do with short hair, while long hair has a lot of versatility. Long hair is known for being luxurious, too.</td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Tom :</b></td>
      <td class = "lowertable" >Short hair is much easier to manage. It’s common for long hair to have a lot of hair damage, such as split ends. With short hair, such problems are easily avoidable. Short hair is simple and clean, while long hair quickly gets messy.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>option</b> 선택 
        </p>
        <p>
          <b>versatility</b> 변하기 쉬움 
        </p>
        <p>
          <b>luxurious</b> 호화로운 
        </p>
        <p>
          <b>manage</b> 관리하다 
        </p>
        <p>
          <b>damage</b> 손상 
        </p>
        <p>
          <b>split end</b> 끝이 갈라진 머리카락 
        </p>
        <p>
          <b>avoidable</b> 피할 수 있는 
        </p>
        <p>
          <b>simple</b> 간단한 
        </p>
        <p>
          <b>clean</b> 깔끔한 
        </p>
        <p>
          <b>messy</b> 지저분한 
        </p>

      </div>

      <div class = "line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr>
            <td class = "uppertable" ><b>제인 :</b></td>
            <td class = "lowertable" >긴 머리가 짧은 머리보다 나아. 왜냐하면 더 많은 스타일링 선택이 있기 때문이야. 짧은 머리로는 할 수 있는 게 많지 않은 반면 긴 머리는 변화하기가 쉬워. 긴 머리도 고급스럽다고 알려져 있어.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>탐 :</b></td>
            <td class = "lowertable" >짧은 머리는 관리하기가 훨씬 쉬워. 긴 머리는 끝이 갈라지는 것과 같은 많은 모발 손상을 입는 것이 일반적이야. 짧은 머리라면, 그러한 문제들은 쉽게 피할 수 있어. 짧은 머리는 단순하고 깔끔한 반면 긴 머리는 금방 지저분해져.</td>
          </tr>
      
          </table>


      </div>

     <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>
            Do you have a long hair or short hair?
          </li>
          <li>Why do you like that haircut?</li>
          <li>In your country, is it common for men to have a long hair? How about for women with short hair?</li>
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
