<template>

    <div :style = "{fontSize: fontSize + 'px'}">
  
      <v-container fluid ma-0 pa-0>
  
        <v-layout column>
          <v-img src="https://image.freepik.com/free-photo/group-portrait-adorable-puppies_53876-64778.jpg" style="max-width: 100%; display:block; height: auto;">
  
          <v-layout
          align-end
          fill-height
          pa-0
          white--text
          >
  
          <transition name="slide-fade">
          <h1 v-if="showTitle" class = "upper-header-lg">Robot Dogs Versus Real Dogs
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
        <td class = "lowertable" >There are so many advancements in technology and they happen very frequently. Robotic dogs, like Aibo, are so lifelike these days that they are great alternatives to actual dogs. Unlike real dogs, however, robot dogs are easier to take care of. Real dogs can be high-maintenance, and many people compare them to babies. Robot dogs come with many characteristics that real dogs have, but you don’t need to feed, clean, or walk them. And since they can’t get sick, there’s no need to take them to a veterinarian.</td>
      </tr>
      <tr class = "second-dialog-lg">
        <td class = "uppertable" ><b>Victoria :</b></td>
        <td class = "lowertable" >Raising a dog can have a positive influence especially on children. Dogs can teach kids the importance of being responsible. According to researchers at Michigan State University, other skills that dog ownership can teach children are trust, compassion, bereavement, respect, self-esteem, loyalty, physical activity, patience, social skills, motivation, and empathy. Robot dogs are toys that are good for bored people who want to be entertained. With a real dog, you learn how valuable life is. Robot dogs, however, aren’t designed to teach you any life skills.</td>
      </tr>
  
      </table>
  
        <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Vocabulary</h3>
  
        <div style="padding : 16px;">
  
          <p>
            <b>alternative</b> 대안
          </p>
          <p>
            <b>high-maintenance</b> 세심한 관리가 필요한
          </p>
          <p>
            <b>characteristic</b> 특징
          </p>
          <p>
            <b>veterinarian</b> 수의사
          </p>
          <p>
            <b>bereavement</b> 사별
          </p>
          <p>
            <b>empathy</b> 감정이입, 공감
          </p>
        </div>
  
        <div class ="line-lg">
        </div>
        <h3 class = "border-translate-lg white--text">해석</h3>
  
        <div style="padding : 16px;">
  
          <table class = "standard-table">
  
            <tr>
              <td class = "uppertable" ><b>David :</b></td>
              <td class = "lowertable" >기술은 많은 발전이 있으며 매우 자주 발생합니다 아이보(Aibo)와 같은 로봇 강아지는 요즘 실제 개들에 대한 훌륭한 대안들이 될 정도로 실제와 같습니다. 하지만 진짜 강아지와 달리 로봇 강아지는 돌보기가 더 쉽습니다. 실제 강아지는 유지 관리가 많을 수 있으며 많은 사람들이 그들을 아기와 비교합니다. 로봇 강아지는 진짜 강아지가 가지고있는 많은 특성을 가지고 있지만 먹이를 주거나 청소하거나 걸을 필요가 없습니다 병에 걸리지 않기 때문에 수의사에게 데려 갈 필요가 없습니다.</td>
            </tr>
            <tr class = "second-dialog-lg">
              <td class = "uppertable" ><b>Victoria :</b></td>
              <td class = "lowertable" >개를 기르는 것은 특히 어린이들에게 긍정적인 영향을 줄 수 있습니다. 개는 아이들에게 책임감의 중요성을 가르칠 수 있습니다. 미시간 주립 대학(Michigan State University)의 연구원에 따르면 개 소유는 아이들에게 가르칠 수 있는 다른 기술은 신뢰, 연민, 사별, 존경, 자존감, 충성도, 신체 활동, 인내, 사회적 기술, 동기 부여 및 공감입니다. 로봇 강아지는 즐거움을 원하는 지루한 사람들에게 좋은 장난감입니다. 진짜 강아지와 함께 여러분은 삶이 얼마나 소중한지 배웁니다. 하지만 로봇 강아지는 여러분에게 어떤 삶의 기술을 가르치도록 고안된 것이 아닙니다.</td>
            </tr>
  
            </table>
  
  
        </div>
  
      <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Questions</h3>
  
        <div style="padding : 16px;">
  
          <ol style="margin: 12px;">
            <li>Have you ever had a pet dog? If not, would you like to?</li>
            <li>Would you consider getting a robot dog as a pet?</li>
            <li>Do you think it’s better to have a real dog or a robot dog? Why?</li>
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
  