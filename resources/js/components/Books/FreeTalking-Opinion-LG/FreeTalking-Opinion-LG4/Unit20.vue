<template>

    <div :style = "{fontSize: fontSize + 'px'}">
  
      <v-container fluid ma-0 pa-0>
  
        <v-layout column>
          <v-img src="https://image.freepik.com/free-photo/child-calculator-finance-copy-space-education_1134-1025.jpg" style="max-width: 100%; display:block; height: auto;">
  
          <v-layout
          align-end
          fill-height
          pa-0
          white--text
          >
  
          <transition name="slide-fade">
          <h1 v-if="showTitle" class = "upper-header-lg">Should Math Be An Optional Course After Elementary School?
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
        <td class = "lowertable" >We learn basic math in elementary school. We learn how to add, subtract, multiply, and divide numbers. We also learn about fractions, shapes, and angles. Do we really need to learn things like the quadratic formula and long division? Unless you’re a mathematician or work with a lot of numbers or shapes, like programmers and architects, we don’t really need to take all these ridiculously advanced math classes. You just need to know simple math to figure out your taxes and how much you should tip someone. </td>
      </tr>
      <tr class = "second-dialog-lg">
        <td class = "uppertable" ><b>Victoria :</b></td>
        <td class = "lowertable" >You might think that math is all about formulas and equations, but it makes you smarter in many ways. According to Dr. Tanya Evans of Stanford University, children who excel in math are able to use their brains much more effectively compared to those who perform poorly. They are able to pay better attention and are better at making decisions. Math helps us to think analytically, too. A lot of the tricky questions that you see on your math exams can actually help you solve a problem in real life.</td>
      </tr>
  
      </table>
  
        <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Vocabulary</h3>
  
        <div style="padding : 16px;">
  
          <p>
            <b>required</b> 필수의
          </p>
          <p>
            <b>algebra</b> 대수학
          </p>
          <p>
            <b>geometry</b> 기하학
          </p>
          <p>
            <b>trigonometry</b> 삼각법
          </p>
          <p>
            <b>calculus</b> 미적분학
          </p>
          <p>
            <b>fraction</b> 분수
          </p>
          <p>
            <b>quadratic formula 2</b> 차 방정식의 근을 푸는 공식
          </p>
          <p>
            <b>long division</b> 장제법
          </p>
          <p>
            <b>architect</b> 건축가
          </p>
          <p>
            <b>ridiculously</b> 터무니 없이
          </p>
          <p>
            <b>formula</b> 공식
          </p>
          <p>
            <b>equation</b> 방정식
          </p>
          <p>
            <b>excel</b> 뛰어나다
          </p>
          <p>
            <b>analytically</b> 분석적으로
          </p>
          <p>
            <b>tricky</b> 까다로운
          </p>

  
        </div>
  
        <div class ="line-lg">
        </div>
        <h3 class = "border-translate-lg white--text">해석</h3>
  
        <div style="padding : 16px;">
  
          <table class = "standard-table">
  
            <tr>
              <td class = "uppertable" ><b>David :</b></td>
              <td class = "lowertable" >우리는 기본적인 수학을 초등학교에서 배웁니다. 우리는 어떻게 숫자를 더하고, 빼고, 곱하고, 나누는지를 배웁니다. 우리는 또한 분수, 도형, 그리고 각에 대해서 배웁니다. 우리는 정말로 근의 공식과 장제법을 배울 필요가 있을까요? 당신이 수학자이거나 프로그래머와 건축가처럼 많은 숫자와 도형과 함께 일을 하지 않는다면 우리는 정말로 이 모든 이상하게 높은 단계의 수학 수업을 들을 필요가 없습니다. 당신은 단지 세금과 팁을 얼마나 주어야 하는지를 계산하기 위한 간단한 수학만 알면 됩니다. </td>
            </tr>
            <tr class = "second-dialog-lg">
              <td class = "uppertable" ><b>Victoria :</b></td>
              <td class = "lowertable" >당신은 수학이 수식과 방정식에 관한 것이라고 생각할 수 있지만, 그것은 당신을 다방면으로 더 똑똑하게 만듭니다. 스텐포드 대학의 타냐 데반스 박사에 따르면 수학에 뛰어난 아이들은 잘 하지 못하는 아이들에 비해 그들의 뇌를 훨씬 더 효과적으로 사용할 수 있습니다. 그들은 집중을 더 잘할 수 있으며 결정을 더 잘 내립니다. 수학은 우리가 분석적으로 사고하는 것 또한 돕습니다. 당신이 수학 시험에서 보는 많은 까다로운 문제들은 사실 실생활에서 문제를 푸는 것을 도와줍니다. </td>
            </tr>
  
            </table>
  
  
        </div>
  
      <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Questions</h3>
  
        <div style="padding : 16px;">
  
          <ol style="margin: 12px;">
            <li>Do you like Mathematics? Why or why not?</li>
            <li>Do you think students should still take advanced Math classes even if they don’t plan to be a programmer, mathematician, or architect?</li>
            <li>Do you find Mathematics useful in your career? Why or why not?</li>
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
  