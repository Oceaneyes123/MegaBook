<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/week-agenda-with-canceled-message_23-2148570708.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is Cancel Culture Good for Society?
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
      <td class = "lowertable" >Cancel culture gives a voice to regular people and those who don’t hold a lot of power. According to Anne Charity Hudley, a professor at the University of California, “Canceling is a way to acknowledge that you don’t have to have the power to change structural inequality. You don’t even have to have the power to change all of public sentiment. But as an individual, you can still have power online.” In other words, we can use social media sites like Twitter to make a change. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Cancel culture is a slippery slope, which is an “idea or course of action which will lead to something unacceptable, wrong, or disastrous,” according to lexico.com. It will lead to intolerance because people will exclude and reject anyone who disagrees with their views. Steven Mintz, a professor at California Polytechnic State University, said, “Some members of the canceling group join in for fear of being canceled themselves. People should be able to speak out or remain silent on the issues without fear of retribution.”</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>structural</b> 구조적인
        </p>
        <p>
          <b>inequality</b> 불평등
        </p>
        <p>
          <b>sentiment</b> 정서
        </p>
        <p>
          <b>intolerance</b> 편협
        </p>
        <p>
          <b>retribution</b> (강력한) 응징[징벌]
        </p>
        
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >캔슬 컬쳐는 일반 사람들과 권력을 많이 가지고 있지 않은 사람들에게 소리를 내게 합니다. 캘리포니아대 교수인 앤 차리티 허들리에 따르면 “취소는 구조적 불평등을 변경할 권한이 필요하지 않다는 것을 인정하는 방법입니다. 대중의 정서를 모두 바꿀 힘도 없어요. 하지만 개인으로서는 여전히 온라인에서 힘을 가질 수 있습니다. 즉, 트위터와 같은 소셜 미디어 사이트를 사용하여 변화를 꾀할 수 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >lexico.com에 따르면, 캔슬 컬처는 미끄러운 경사면이며, 이것은 "용납할 수 없거나, 잘못되고, 또는 비참한 일로 이어질 생각이나 행동 과정"이라고 합니다." 사람들은 자신의 견해에 동의하지 않는 사람을 배제하고 거부하기 때문에 편협으로 이어질 것입니다. 캘리포니아 폴리테크닉 주립대 교수인 스티븐 민츠는 "취소하는 그룹의 일부 구성원들이 스스로 취소될까 봐 참여하는 경우도 있다"고 말했습니다. 사람들은 보복에 대한 두려움없이 문제에 대해 말하거나 침묵을 유지할 수 있어야합니다.”</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you heard about “Cancel Culture”? If no, what do you think is it about?</li>
          <li>Do you think it’s okay to “cancel” a person because they have a different opinion from the rest?</li>
          <li>Is cancel culture unfair? Why or why not?</li>
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
