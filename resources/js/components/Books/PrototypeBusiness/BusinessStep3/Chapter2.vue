<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGvzS3QfY/6/screen_2x/canva-brown-monkey-toy-MADGvzS3QfY.jpg" class = "cover-photo"> 

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
        padding-bottom: 10px;">Talking about products and services</h1>
    </v-layout>
  </v-img>

  <div style=" border-color:#402B24; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border white--text" >Today's topic</h3>
  <div style = "padding : 16px;">


    <p>
      A salesman from a company called Fun Farm is talking to a potential customer at a trade fair.<br />
      </p>
      <br />

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
  
        <p>
          Fun Farm이라는 회사의 세일즈맨이 무역 박람회에서 잠재 고객과 이야기를 나누고 있다.<br />
          </p>
          <br />

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
            What does Fun Farm manufacture?
          </li>
          <li>
            What's the woman's job?
          </li>
          <li>
            Where does Fun Farm make its products?
          </li>
        </ol>

        <p>
           Talk about the products and services of a company you know well.
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
                  Be - <b>Is</b> the trade fair in Montreal?<br />
                  &emsp;&emsp;Where <b>are</b> your offices?
                </p>
                <p>
                  Other verbs – When <b>does</b> the fair start?<br />
                  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;<b>Do</b> they make computers?
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
          name:'Woman:',
          speech:'So you make plastic animals.'
        },
        {
          name:'Representative:',
          speech:'That’s right. All life-size. Cows, horses, sheep...'
        },
        {
          name:'Woman:',
          speech:'They’re very realistic... Oh, and they move!'
        },
        {
          name:'Representative:',
          speech:'Their heads move. They make sounds, if you just touch them...'
        },
        {
          name:'Woman:',
          speech:'Oh!'
        },
        {
          name:'Representative:',
          speech:'They don’t walk! Our customers prefer them to stay in one place.'
        },
        {
          name:'Woman:',
          speech:'Yes, right. So who are your customers? Where do you sell these things?'
        },
        {
          name:'Representative:',
          speech:'We sell a lot to fun parks, shopping centres, playgrounds... Children all over the world love them. We export to twenty-five countries.'
        },
        {
          name:'Woman:',
          speech:'Really? I manage a small fun park in Germany. It’s for children up to twelve years old.'
        },
        {
          name:'Representative:',
          speech:'Well, they are perfect for that age. We have a lot of customers in Germany. We work with a company called DDA, in Frankfurt. They install our products, and look after maintenance and after-sales service for all our German customers.'
        },
        {
          name:'Woman:',
          speech:'Right. So what country are you from?'
        },
        {
          name:'Representative:',
          speech:'From Canada. We have a factory near Montreal. We manufacture all our products there.'
        },
        {
          name:'Woman:',
          speech:'Oh, I see... Can I just...?'
        },
        {
          name:'Representative:',
          speech:'Sure.'
        },
        ],

        translations:[
        {
          name:'W:',
          speech:'그럼 당신은 플라스틱 동물을 만드는군요.'
        },
        {
          name:'대표자:',
          speech:'맞아요. 모든 실물 크기. 소, 말, 양...'
        },
        {
          name:'W:',
          speech:'그들은 정말 현실적이에요... 오, 그리고 그들은 움직여요!'
        },
        {
          name:'대표자:',
          speech:'그들의 머리는 움직입니다. 소리가 나는데 만지면...'
        },
        {
          name:'W:',
          speech:'오!'
        },
        {
          name:'대표자:',
          speech:'그들은 걷지 않아요! 우리의 고객들은 그들이 한 곳에 머무르는 것을 선호합니다.'
        },
        {
          name:'W:',
          speech:'그래, 맞아요. 그래서 당신의 고객은 누구인가요? 이 물건들은 어디서 파십니까?'
        },
        {
          name:'대표자:',
          speech:'우리는 재미있는 공원, 쇼핑 센터, 놀이터에 많은 것을 팝니다... 전 세계의 어린이들은 그들을 사랑합니다. 우리는 25개국에 수출합니다.'
        },
        {
          name:'Wo:',
          speech:'그래요? 나는 독일에서 작은 재미난 공원을 운영합니다. 12세까지의 어린이를 위한 겁니다.'
        },
        {
          name:'대표자:',
          speech:'글쎄, 그 나이에 딱 맞는 것이 있어요. 독일에는 손님이 많아요. 우리는 프랑크푸르트에 있는 DDA라는 회사와 함께 일합니다. 그들은 우리의 제품을 설치하고, 우리의 모든 독일 고객들을 위해 유지 보수와 애프터서비스를 돌봅니다.'
        },
        {
          name:'W:',
          speech:'그렇군요. 그래서 당신은 어느 나라에서 왔나요?'
        },
        {
          name:'대표자:',
          speech:'캐나다에서요. 우리는 몬트리올 근처에 공장이 있습니다. 우리는 그곳에서 모든 제품을 생산합니다.'
        },
        {
          name:'W:',
          speech:'아, 그렇구나... 제가 그냥…?'
        },
        {
          name:'대표자:',
          speech:'물론이죠.'
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
