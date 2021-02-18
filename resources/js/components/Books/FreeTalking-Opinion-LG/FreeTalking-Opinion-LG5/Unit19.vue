<template>

    <div :style = "{fontSize: fontSize + 'px'}">
  
      <v-container fluid ma-0 pa-0>
  
        <v-layout column>
          <v-img src="https://image.freepik.com/free-photo/cyber-monday-shopping-sales_23-2148688507.jpg" style="max-width: 100%; display:block; height: auto;">
  
          <v-layout
          align-end
          fill-height
          pa-0
          white--text
          >
  
          <transition name="slide-fade">
          <h1 v-if="showTitle" class = "upper-header-lg">Should All Shopping Be Online?
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
        <td class = "lowertable" >Online shopping is the future, and we should invest in the future. Although one could go to the store and purchase certain items, there is always a chance that the store has run out of stock. In contrast, the internet is a wide growing marketplace, with the ability to access and purchase items from across the globe. We all have internet connections, and the ease-of-use and comfort and speed of delivery is something too good to pass up. By handling shopping through online means, we have more time to focus on things that really matter.</td>
      </tr>
      <tr class = "second-dialog-lg">
        <td class = "uppertable" ><b>Victoria :</b></td>
        <td class = "lowertable" >Online shopping ruins multiple industries. It is currently ruining the distribution outlets of many stores and small businesses. While these stores may have online capabilities, they do not have the wide choice of items and shipping and delivery logistics like the big stores. Furthermore, with the research of drones for delivery, online shopping will start to hamper the delivery industry and cost many people their jobs. Online shopping is more convenient, but it cuts away at human interaction. We should still make normal shopping available, lest we have more haggard shut-ins.</td>
      </tr>
  
      </table>
  
        <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Vocabulary</h3>
  
        <div style="padding : 16px;">
  
          <p>
            <b>in contrast</b> 그에 반해서
          </p>
          <p>
            <b>pass up</b> (기회 등을) 거절하다
          </p>
          <p>
            <b>currently</b> 현재, 지금
          </p>
          <p>
            <b>distribution</b> 유통
          </p>
          <p>
            <b>outlet</b> (특정 회사의 것이나 특정 유형의 상품을 취급하는) 직판점
          </p>
          <p>
            <b>logistics</b> 물류
          </p>
          <p>
            <b>hamper</b> 방해하다
          </p>
          <p>
            <b>interaction</b> 상호작용
          </p>
          <p>
            <b>lest</b> ~하지 않도록
          </p>
          <p>
            <b>haggard</b> 초췌한
          </p>
  
        </div>
  
        <div class ="line-lg">
        </div>
        <h3 class = "border-translate-lg white--text">해석</h3>
  
        <div style="padding : 16px;">
  
          <table class = "standard-table">
  
            <tr>
              <td class = "uppertable" ><b>David :</b></td>
              <td class = "lowertable" >온라인 쇼핑은 미래이며 우리는 미래에 투자해야 합니다. 비록 가게에 가서 특정한 상품들을 살 수 있지만, 그 가게에서 재고가 떨어질 가능성은 항상 있습니다. 대조적으로, 인터넷은 성장하고 있는 광범위한 시장이며 전 지구에서 물품들에 접근하고 구매할 수 있는 능력을 갖고 있습니다. 우리는 모두 인터넷에 연결되어 있으며, 사용의 용이함과 배달의 편리함과 속도는 그냥 지나치기엔 너무나 좋은 것입니다. 온라인 수단을 통해 쇼핑을 다룸으로써, 우리는 정말로 중요한 것들에게 집중할 더 많은 시간을 가질 수 있습니다. </td>
            </tr>
            <tr class = "second-dialog-lg">
              <td class = "uppertable" ><b>Victoria :</b></td>
              <td class = "lowertable" >온라인 쇼핑은 다수의 산업을 망칩니다. 이것은 현재 많은 가게와 소규모 사업체의 분배 수단을 망치고 있습니다. 이러한 가게들이 온라인 능력을 가질 수 있지만, 이것들은 큰 가게들처럼 상품의 넓은 선택권, 운송과 배달 물류 실행 계획을 가지고 있지 않습니다. 더욱이, 배달을 위한 무인항공기 연구로 온라인 쇼핑은 배달 산업을 방해하고 많은 사람들에게서 직장을 빼앗기 시작할 것입니다. 온라인 쇼핑은 더욱 편리하지만, 인간의 상호작용을 차단합니다. 우리가 초췌하며 바깥 출입을 못하는 사람들을 더 가지지 않도록 평범한 쇼핑을 여전히 이용 가능하게 해야 합니다. </td>
            </tr>
  
            </table>
  
  
        </div>
  
      <div class = "line-lg">
        </div>
        <h3 class = "border-lg white--text">Questions</h3>
  
        <div style="padding : 16px;">
  
          <ol style="margin: 12px;">
            <li>Do you like to shop online? Why or why not?</li>
            <li>With everything available online, what items do you think must still be purchased on physical stores?</li>
            <li>What do you think would happen if all shopping transactions would be made online?</li>
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
  