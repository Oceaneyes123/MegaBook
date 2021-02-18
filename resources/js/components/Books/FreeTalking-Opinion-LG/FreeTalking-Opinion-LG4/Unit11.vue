<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/close-up-cute-french-bulldog-lying-shoulder-her-female-owner-picture-from-back-female-veterinarian-pressing-sad-puppy-her-while-doing-tests-relation-responsibility_176420-11055.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Animal Testing Be Banned?
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
      <td class = "lowertable" >Animals used in experiments are commonly subjected to terrible conditions. According to Humane Society International, they are often killed by carbon dioxide asphyxiation, neck-breaking, and decapitation. In addition, these animals go through forced feeding, food and water deprivation, long periods of physical restraint, and infliction of pain for the sake of research. A study in the Brazilian Archives of Biology and Technology states that many cosmetic companies use something called the Draize eye test to assess their products. It involves rabbits having their eyelids forced open for multiple days.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Since animals are similar to humans in many ways, they are appropriate research subjects. According to the California Biomedical Research Association, chimpanzees share 99 percent of their DNA with people, while mice are 98 percent genetically similar to us. Furthermore, all mammals are descended from common ancestors, so we all have the same organs and they function the same way. Plus, animalresearch.info states that animals themselves benefit from the results of animal testing. Vaccines help both humans and animals, and even pacemakers exist because of animal testing.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>commercial</b> 상업의
        </p>
        <p>
          <b>asphyxiation</b> 질식
        </p>
        <p>
          <b>decapitation</b> 참수, 목 베기
        </p>
        <p>
          <b>deprivation</b> 박탈
        </p>
        <p>
          <b>infliction</b> (고통·벌·타격을) 가함[줌]
        </p>
        <p>
          <b>assess</b> 평가하다
        </p>
        <p>
          <b>pacemaker</b> pacemaker
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >실험에 사용 된 동물은 대개 끔찍한 조건을 겪습니다. 휴메인 소사이어티 인터내셔널에 따르면, 그들은 종종 이산화탄소 질식, 목꺾기, 그리고 목이 매여 죽임을 당합니다. 또한 이 동물들은 강제 섭식, 식량과 물 부족, 오랜 기간의 신체적 구속 및 연구를 위한 고통의 가중을 겪습니다. 브라질 생물 기술 학술지의 한 연구는 많은 화장품 회사가 그들의 제품을 평가하기 위하여 드레이즈 눈 테스트라고 불리는 무언가를 이용한다는 것을 주장합니다. 그것은 눈꺼풀을 여러 날 동안 열어 놓은 토끼에 관련된 것입니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >동물들은 여러 면에서 인간과 유사하기 때문에 적절한 연구 주제입니다. 캘리포니아 생물 의학 연구 협회에 따르면, 침팬지는 인간 DNA와 99 %의 DNA를 공유하는 반면 쥐는 우리와 유전적으로 유사합니다. 게다가 모든 포유류는 공통 조상에서 유래되었으므로 우리 모두는 같은 장기를 가지며 같은 방식으로 기능합니다. 또한 animalresearch.info는 동물 자체가 동물 실험의 결과로부터 이익을 얻는다고 말합니다. 백신은 인간과 동물 모두에게 도움이 되며, 동물 실험 때문에 심지어 페이스 메이커도 존재합니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you consider animal testing cruel and inhumane? Why or why not?</li>
          <li>What difference would it make if researchers never implemented animal testing?</li>
          <li>Do you think it is only right for animal testing to be banned? Why or why not?</li>
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
