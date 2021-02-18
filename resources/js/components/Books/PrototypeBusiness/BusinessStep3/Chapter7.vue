<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADQ5BePL5w/1/screen_2x/canva-vacuum-cleaner-on-a-wooden-floor-MADQ5BePL5w.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgba(140, 103, 90, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Comparing offers 
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color:#402B24; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border white--text" >Today's topic</h3>
  <div style = "padding : 16px;">

  
    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table> 


    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #402B24; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #402B24;">Translation</h3>
    <div style="padding : 16px;">

      <table style = "border-collapse: collapse;">

        <tr v-for="translation in translations" :key="translation">
          <td class = "uppertable" >{{translation.name}}</td>
          <td class = "lowertable" >{{translation.speech}}</td>
        </tr>

      </table>
   </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Exercise</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>
            Is there much difference between the quality of the products?
          </li>
          <li>
            What’s the main difference between the products?
          </li>
          <li>
            What does Marilyn think of the Aerosaurus?
          </li>
          <li>
            What does Lionel think of the Aerosaurus?
          </li>
        </ol>

        <p>
           Free response:<br />
           Compare the price and quality of pairs of competing products and stores you both know.<br />
           - mobile phones<br />
           - supermarkets<br />
           - clothes shops<br />
           ...is much cheaper, but the quality isn't as good... .<br />
           ...sells better quality products than ... .<br />
        </p>

      </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Self Study</h3>
      <div style="padding : 16px;">


          <p>
            Notes
          </p>

        <p>

          <v-container grid-list-md text-xs-left>
            <v-layout row wrap>


              <v-flex xs12>
                <v-card light color="#F2CBBD">
                  <v-card-text class="px-10">
                <p>
                  Comparatives<br />
                  Short adjectives : It’s often fast<b>er</b> and cheap<b>er</b> to buy online.<br />
                  Long adjectives : (+) BMWs are a lot <b>more</b> expensive <b>than</b> Skodas.<br />
                  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp; (-) Skodas are a lot<b>less</b> expensive <b>than</b> BMWs.<br />
                  Irregular adjectives : The situation is <b>worse/better</b> now.<br />
                  As…as : This one isn’t <b>as</b> popular <b>as</b> the other one.
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
          name:'Lionel:',
          speech:'Marilyn, these are both top quality products! The quality is the same.'
        },
        {
          name:'Marilyn:',
          speech:'I know. But they don’t look the same. The one from Gild looks like a modern vacuum cleaner. This Aero…'
        },
        {
          name:'Lionel:',
          speech:'Aerosaurus.'
        },
        {
          name:'Marilyn:',
          speech:'Yeah. It looks like something from the 1960s.'
        },
        {
          name:'Lionel:',
          speech:'Well of course it does. It’s a retro look.'
        },
        {
          name:'Marilyn:',
          speech:'I know, but what do most customers want? Do they want to pay a reasonable price for a modern vacuum cleaner, or pay more for something that looks forty years old?'
        },
        {
          name:'Lionel:',
          speech:'Yes, but surely we don’t want just another ‘modern’ vacuum cleaner, that’s the same as all the other products we sell? We need something different. OK, the Aerosaurus is more expensive. But it’s different… And Suntra is making a good offer. Look ? twelve percent discount - Gild is only offering five percent. Suntra is offering cheaper delivery, as well. We can make a bigger profit margin.'
        },
        {
          name:'Marilyn:',
          speech:'We can make a bigger margin, but we can only make a good profit if we sell enough vacuum cleaners. How many of these Aero…sauruses can we sell? I mean, look at it. It looks like a dinosaur!'
        },
        {
          name:'Lionel:',
          speech:'Of course it does! That’s why people will love it! Just listen to it!'
        },
        ],


        translations:[
        {
          name:'리오넬:',
          speech:'마릴린, 둘 다 최고 품질의 제품입니다! 퀄리티가 똑같아요.'
        },
        {
          name:'마릴린:',
          speech:'알아요 하지만 그들은 같지 않습니다. Gild에서 나온 것은 현대식 진공 청소기처럼 보입니다. 이 에어로는 …'
        },
        {
          name:'리오넬:',
          speech:'에어로사우루스입니다.'
        },
        {
          name:'마릴린:',
          speech:'네, 1960년대 것 같아요.'
        },
        {
          name:'리오넬:',
          speech:'물론 그렇습니다. 복고풍이에요..'
        },
        {
          name:'마릴린:',
          speech:'알아요, 그런데 대부분의 고객이 원하는 게 뭐죠? 그들은 현대식 진공청소기에 적당한 가격을 지불하길 원하나요, 아니면 40년 된 것 같은 것에 더 많은 돈을 지불하길 원하나요?'
        },
        {
          name:'리오넬:',
          speech:'네, 하지만 우리가 파는 다른 모든 제품과 똑같은 ’현대식’ 청소기를 또 원하는 건 아니겠죠? 우리는 뭔가 다른 것이 필요합니다. 좋아요, 에어로사우루스가 더 비싸요. 하지만 그것은 다릅니다. 그리고 선트라는 좋은 제안을 하고 있습니다. 보세요? 12퍼센트 할인된 가격 - Gild는 단지 5%만 할인하고 있습니다. 선트라는 또한 더 저렴한 배송을 제공하고 있습니다. 우리는 더 큰 이윤을 낼 수 있습니다.'
        },
        {
          name:'마릴린:',
          speech:'더 큰 마진은 벌 수 있지만, 진공청소기를 충분히 팔아야만 좋은 수익을 낼 수 있습니다. 이 에어로 사우루스 중 몇 개를 팔 수 있습니까? 제 말은, 이것 좀 보세요. 그것은 공룡처럼 생겼어요!'
        },
        {
          name:'리오넬:',
          speech:'물론 그렇습니다! 그래서 사람들이 그것을 좋아할 거예요! 그냥 들어보세요!'
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
  border-color: transparent#402B24 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background:#402B24;
  padding-left: 10px;

}
.profile {
  background-color: rgba(0, 0, 0, 0);
  width: 100%;
  padding-top : 330px;
  padding-left : 10px;
  padding-bottom: 10px;
}

.uppertable {
  border: 0px solid #dddddd;
  text-align: left; padding: 8px;
  vertical-align:top;
  width: 5%;
  white-space: nowrap;
}

.lowertable {
  border: 0px solid #dddddd;
  text-align: left;
  padding: 8px;
}

</style>
