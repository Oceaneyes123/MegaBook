<template>

    <div :style = "{fontSize: fontSize + 'px'}">
  
      <v-container fluid ma-0 pa-0>
  
        <v-layout column>
          <v-img src="https://image.freepik.com/free-photo/woman-checking-calendar_53876-13451.jpg" style="max-width: 100%; display:block; height: auto;">
  
          <v-layout
          align-end
          fill-height
          pa-0
          white--text
          >
  
          <transition name="slide-fade">
          <h1 v-if="showTitle" class = "upper-header-lg">Should we stop celebrating unofficial holidays?
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
        <td class = "lowertable" >Pepero Day, White Day, you name it. Korea has a day for almost anything trivial or special, and I think the country’s consumption culture has reached an uncontrollable level in which people spend way too much on chocolates, roses, and other gifts. Companies fan this materialistic culture because they make people think that only through the products they sell can messages of love, appreciation, or congratulations be relayed. I believe that small gestures or acts of kindness are more meaningful than gifts.</td>
      </tr>
      <tr class = "second-dialog-lg">
        <td class = "uppertable" ><b>Victoria :</b></td>
        <td class = "lowertable" >I personally don’t mind spending money to buy small gifts for my loved ones and friends on these occasions. First of all, it’s not every day we celebrate these things and imagine the happiness a gift can bring when you surprise someone with Pepero or a rose. For me, that is priceless. Second, the products we purchase make the occasion extra special because that way, they leave a physical memory or remembrance of when you brightened up someone’s day and made them smile.</td>
      </tr>
  
      </table>
  
        <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Vocabulary</h3>
  
        <div style="padding : 16px;">
  
          <p>
            <b>trivial</b> 사소한
          </p>
          <p>
            <b>uncontrollable</b> 통제할 수 없는
          </p>
          <p>
            <b>materialistic</b> 물질주의적인
          </p>
          <p>
            <b>appreciation</b> 감사
          </p>
          <p>
            <b>congratulation</b> 축하
          </p>
          <p>
            <b>relay</b> 전달하다
          </p>
          <p>
            <b>gesture</b> 표현
          </p>
          <p>
            <b>brighten up</b> 밝게 하다
          </p>
        </div>
  
        <div class ="line-lg">
        </div>
        <h3 class = "border-translate-lg white--text">해석</h3>
  
        <div style="padding : 16px;">
  
          <table class = "standard-table">
  
            <tr>
              <td class = "uppertable" ><b>David :</b></td>
              <td class = "lowertable" >빼빼로 데이, 화이트 데이 그 밖에 무엇이든지. 한국은 사소한 혹은 특별한 어떤 것이든 거의 기념이 존재하며 저는 이 나라의 소비 문화가 사람들이 초콜렛과 장미 그리고 다른 선물에 너무 많이 소비를 하는 통제할 수 없는 단계에 접어들었다고 생각합니다. 기업들은 사람들이 오로지 그들이 파는 상품을 통해서만 사랑과, 감사 그리고 축하의 메시지를 전달 수 있다고 생각하게 만들기에 물질주의적인 문화를 부채질하고 있습니다. 저는 친절함의 작은 손짓이나 행동이 선물보다 더 가치가 있다고 믿습니다.</td>
            </tr>
            <tr class = "second-dialog-lg">
              <td class = "uppertable" ><b>Victoria :</b></td>
              <td class = "lowertable" >저는 개인적으로 기념일에 사랑하는 사람들이나 친구들을 위해 작은 선물을 사는 데 돈을 소비하는 것을 별로 꺼리지 않습니다. 무엇보다, 우리가 매일 이러한 것들을 축하하고 당신이 누군가를 빼빼로나 장미로 놀래킬 때 선물이 가져다 주는 행복을 상상하는 것이 아닙니다. 저는 그것의 값어치를 매길 수 없습니다. 두 번째로, 우리가 구매하는 상품들은 당신이 누군가의 하루를 밝게 하고 웃게 만들었다는 물리적인 기억이나 추억을 남기기에 기념임을 더 특별하게 만듭니다.</td>
            </tr>
  
            </table>
  
  
        </div>
  
      <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Questions</h3>
  
        <div style="padding : 16px;">
  
          <ol style="margin: 12px;">
            <li>Do you also celebrate unofficial holidays? If yes, which ones do you usually celebrate?</li>
            <li>Do you have a favorite holiday? If yes, what is it and why?</li>
            <li>If you were to create an unofficial holiday, what would it be and why?</li>
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
  