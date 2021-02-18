<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGxjjkvao/5/screen_2x/canva-white-blue-and-green-t-shirt-shaped-banknote-MADGxjjkvao.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgba(254, 183, 43, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing sales and orders
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border" >Today's topic</h3>
  <div style = "padding : 16px;">


    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table>

    
    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Translation</h3>
    <div style="padding : 16px;">

      <table style = "border-collapse: collapse;">

        <tr v-for="translation in translations" :key="translation">
          <td class = "uppertable" >{{translation.name}}</td>
          <td class = "lowertable" >{{translation.speech}}</td>
        </tr>

      </table>
   </div>


   
    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Exercise</h3>
    <div style="padding : 16px;">

      <p>
        Make questions with much or many.
      </p>

      <ol style="margin: 12px;">
        <li>
           how/ products/ are on sale?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          how/ profit/ did you make?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          how/discount/ did you get?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
      </ol>
      <p>
        Free response:<br />
        Talk about a market/industry from the box(or one you know well).
      </p>
      <u>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;</u>
      <p>
        food    soft drinks    mobile    clothes/fashion
      </p>
      <u>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;</u>
      <p>
        What's the biggest company in the market?<br />
        Who are the company's competitors?<br />
        Is the market very competitive?<br />
        Is demand increasing or decreasing?
      </p>

    </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Self Study</h3>
    <div style="padding : 16px;">


      <p>
        Notes
      </p>

      <p>

        <v-container grid-list-md text-xs-left>
          <v-layout row wrap>


            <v-flex xs12>
              <v-card light color="#527318">
                <v-card-text class="px-10">
                  <p>
                    much/many:questions
                  </p>
                  <p>
                    셀 수 있는 명사 How <b>many</b> stores do you have?<br />
                    셀 수 없는 명사 How <b>much</b> discount is there?
                  </p>
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>

      </p>

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
      dialogs:[
        {
          name:'A:',
          speech:'So how many T-shirts did we order?'
        },
        {
          name:'B:',
          speech:'Um...two thousand five hundred.'
        },
        {
          name:'A:',
          speech:'Right. So it’s quite a small order, then.'
        },
        {
          name:'B:',
          speech:'Yeah. It’s a new product, so we want to test it first.'
        },
        {
          name:'A:',
          speech:'Sure. How many stores are we selling them in?'
        },
        {
          name:'B:',
          speech:'Five.'
        },
        {
          name:'A:',
          speech:'Right. And do you know the selling price?'
        },
        {
          name:'B:',
          speech:'They’re on sale at nine euros, in the stores. It’s a cheap product.'
        },
        {
          name:'A:',
          speech:'Hmm. Are we making much profit on them?'
        },
        {
          name:'B:',
          speech:'On this order, forty percent.'
        },
        {
          name:'A:',
          speech:'And what about bigger orders? How much discount can we get?'
        },
        {
          name:'B:',
          speech:'Ten or fifteen percent more.'
        },
        {
          name:'A:',
          speech:'So we can make a fifty, fifty-five percent profit margin on them?'
        },
        {
          name:'B:',
          speech:'Yeah. And more, if they sell well. I think we can get a maximum twenty percent discount on really big orders.'
        },
        {
          name:'A:',
          speech:'Is there much demand at the moment? That’s the question. Do many people want to buy T-shirts in winter?'
        },
        {
          name:'B:',
          speech:'Well, people buy them to wear under sweaters and shirts...'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'티셔츠를 몇 벌이나 주문했나요?'
        },
        {
          name:'B:',
          speech:'음...2천5백개요.'
        },
        {
          name:'A:',
          speech:'그렇군요. 그렇다면 꽤 작은 주문이네요.'
        },
        {
          name:'B:',
          speech:'네. 신제품이라 먼저 테스트해 보고 싶어요.'
        },
        {
          name:'A:',
          speech:'물론이죠. 몇 개 매장에서 팔지?'
        },
        {
          name:'B:',
          speech:'다섯 개요.'
        },
        {
          name:'A:',
          speech:'그렇군요. 그리고 당신은 판매 가격을 알고 있나요?'
        },
        {
          name:'B:',
          speech:'매장에서 9유로로 판매되요. 싼 가격의 제품이다.'
        },
        {
          name:'A:',
          speech:'H흠. 우리가 그들에게서 많은 이익을 내고 있는 건가요?'
        },
        {
          name:'B:',
          speech:'이번 주문의 40%.'
        },
        {
          name:'A:',
          speech:'그럼 더 큰 주문은 어쩌고요? 얼마나 할인을 받을 수 있을까요?'
        },
        {
          name:'B:',
          speech:'10~15% 정도 더요.'
        },
        {
          name:'A:',
          speech:'그럼 55퍼센트의 이윤을 낼 수 있는 건가요?'
        },
        {
          name:'B:',
          speech:'네. 그리고 잘 팔리면 더 많이. 정말 큰 주문은 최대 20%까지 할인받을 수 있을 것 같아요.'
        },
        {
          name:'A:',
          speech:'지금 수요가 많나요? 그게 문제입니다. 많은 사람들이 겨울에 티셔츠를 사고 싶어할까요?'
        },
        {
          name:'B:',
          speech:'음, 사람들은 스웨터와 셔츠를 입기 위해 그것들을 삽니다.'
        },
        {
          name:'A:',
          speech:'음, 사람들은 스웨터와 셔츠를 입기 위해 그것들을 삽니다.'
        },
        ]

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

.border:before {
  content: "";
  width: 0px;
  height: 0px;
  border-style: solid;
  border-width: 40px 40px 0px 0px;
  transform: rotate(180deg);
  border-color: transparent #899857 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background: #899857;
  padding-left: 10px;

}
.profile {
  background-color: rgba(0, 0, 0, 0);
  width: 100%;
  padding-top : 330px;
  padding-left : 10px;
  padding-bottom: 10px;
}


</style>
