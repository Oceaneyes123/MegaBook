<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/day-view-prague_1398-2773.jpg" class="cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgb(59, 105, 120, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">I'd like to visit Europe
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">I'd like to visit Europe</li><br />

      <br />
      <p>
        Mr. and Mrs. Thompson would like to visit Europe this summer. At the moment, they’re talking to their travel agent, Mr. Winkle.<br />
      </p>
      <br />

      <table style = "border-collapse: collapse;">
    
        <tr v-for="dialog in dialogs" :key="dialog">
          <td class = "uppertable" >{{dialog.name}}</td>
          <td class = "lowertable" >{{dialog.speech}}</td>
        </tr>
  
      </table>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;
                                              margin-left: -18px;
                                              margin-right: -18px;
                                              padding-left: 10px;
                                              padding-bottom: 10px;
                                              padding-top: 10px;
                                              margin-top: 0px;
                                              background-color: #204051;">Exercise</h3>
        <div style="padding : 16px;">

        <p>
          <u>Answer the questions</u><br />
        </p>

        <ol style="margin: 12px;">
          <li>
            What would Mr. and Mrs. Thompson like to do this summer?<br />
          </li>
          <li>
            Do the Thompson’s need a translator? Why?<br />
          </li>
          <li>
            How much is the deposit for the tour?<br />
          </li>
          <li>
            Would you like to visit Europe?<br />
          </li>
          <li>
            Which countries would you like to visit?<br />
          </li>
        </ol>

      </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;
                                              margin-left: -18px;
                                              margin-right: -18px;
                                              padding-left: 10px;
                                              padding-bottom: 10px;
                                              padding-top: 10px;
                                              margin-top: 0px;
                                              background-color: #204051;">Translation</h3>
      <div style="padding : 16px;">

        <p>
          Thompson 부부는 이번 여름에 유럽을 방문하고 싶어 합니다. 지금, 그들은 여행사 직원인 Winkle씨와 이야기를 나누고 있습니다.<br />
        </p>

        <table style = "border-collapse: collapse;">

          <tr v-for="translation in translations" :key="translation">
            <td class = "uppertable" >{{translation.name}}</td>
            <td class = "lowertable" >{{translation.speech}}</td>
          </tr>
  
        </table>

</div>
        <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
        </div>
        <h3 class = "border white--text" style="padding-top: 7px;
                                                margin-left: -18px;
                                                margin-right: -18px;
                                                padding-left: 10px;
                                                padding-bottom: 10px;
                                                padding-top: 10px;
                                                margin-top: 0px;
                                                background-color: #204051;">Self Study</h3>
        <div style="padding : 16px;">

          <p>

            <v-container grid-list-md text-xs-left>
              <v-layout row wrap>


                <v-flex xs12>
                  <v-card light color="#cae8d5">
                    <v-card-text class="px-10">
                    <li>
                      Notes
                    </li>
                    <ol style="margin: 12px;">
                    <li>
                        would like to + verb : 소망을 의미하는 표현으로 '~하고 싶다'는 뜻입니다. want와 같은 의미입니다. 정중하게 제안할 때도 쓰입니다.<br />
                            Ex) Thompson would like to visit Europe this summer : Thompson은 올 여름에 유럽을 방문하고 싶어한다<br />
                            I would like to know more about the hotels : 그 호텔에 대해서 더 알고 싶다<br />
                    </li>
                    <li>
                      each : 각각의, 각자의, 단수취급하여 뒤에 오는 명사도 단수를 써줍니다.<br />
                    </li>
                    <li>
                      to부정사 : 감정을 나타내는 형용사 뒤의 to부정사는 감정의 원인을 나타내며, ~해서라고 해석합니다. You'll be happy to know..: 알아서 기쁠 것이다.<br />
                    </li>
                    <li>
                      at the moment : 바로 지금<br />
                    </li>
                    <li>
                      perfect for you : 너에게 완벽하다<br />
                    </li>
                    <li>
                      all of Europe : 전 유럽<br />
                    </li>
                    <li>
                      free time in each country : 각 나라에서 자유시간을<br />
                    </li>
                    <li>
                      stay in (장소): ~에 머무르다<br />
                    </li>
                    <li>
                      famous for : ~때문에 유명하다<br />
                    </li>
                    <li>
                      at no extra charge : 할증수수료 없이<br />
                    </li>
                    <li>
                      worry about ~ : ~에 대해 걱정하다<br />
                    </li>
                    <li>
                      help you with anything you need : 당신이 필요한 것이면 무엇이든지 돕다<br />
                    </li>
                    </ol>
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
          name:'Winkle:',
          speech:'We have three European tours. Our Grand Tour will be perfect for you. Would you like to see our brochure?'
        },
        {
          name:'Thompson:',
          speech:'Yes, we would. These pictures are lovely. Will the tour include all of Europe, Mr. Winkle?'
        },
        {
          name:'W:',
          speech:'Of course. And you’ll have a lot of free time in each country.'
        },
        {
          name:'T:',
          speech:'I would like to know more about the hotels. Are they first-class?'
        },
        {
          name:'W:',
          speech:'Naturally. You’ll stay in the best hotels in Europe. They all have great locations, excellent rooms and fine cuisine.'
        },
        {
          name:'T:',
          speech:'Tell us more about the food. We like to eat well.'
        },
        {
          name:'W:',
          speech:'You’ll be happy to know all the restaurants on the Grand Tour are famous for their cuisine. You can dine when and where you like, even in your room. At no extra charge.'
        },
        {
          name:'T:',
          speech:'What about tipping? Is the service included?'
        },
        {
          name:'W:',
          speech:'You don’t have to worry about tipping. The tour manager pays all the waiters, drivers and guides.'
        },
        {
          name:'T:',
          speech:'Can the tour manager translate for us? We don’t speak any foreign languages.'
        },
        {
          name:'W:',
          speech:'All the tour managers speak several languages. They can help you with anything you need.'
        },
        {
          name:'T:',
          speech:'That’s wonderful.'
        },
        {
          name:'W:',
          speech:'Shall I make your reservations now?'
        },
        {
          name:'T:',
          speech:'Yes. Would you like a deposit?'
        },
        {
          name:'W:',
          speech:'Yes, thank you. That will be $500. I know you’ll enjoy your trip.'
        },
        ],

        translations:[
        {
          name:'Winkle:',
          speech:'유럽 투어는 세 번 있습니다. 우리의 그랜드 투어는 당신에게 완벽할 것입니다. 저희 책자를 보시겠어요?'
        },
        {
          name:'Thompson:',
          speech:'그 이유는 다음과 같습니다. 네, 그럴 거예요. 이 사진들은 사랑스러워요. 이 투어에는 유럽 전역이 포함되나요, Winkle 씨?'
        },
        {
          name:'W:',
          speech:'물론이죠. 그리고 각 나라마다 자유시간이 많을 것입니다.'
        },
        {
          name:'T:',
          speech:'호텔에 대해 더 알고 싶습니다. 그들은 일등석인가요?'
        },
        {
          name:'W:',
          speech:'당연하죠. 당신은 유럽에서 가장 좋은 호텔에서 머물 것입니다. 그들은 모두 훌륭한 장소와 훌륭한 방, 그리고 훌륭한 요리를 가지고 있습니다.'
        },
        {
          name:'T:',
          speech:'음식에 대해 더 말해주세요. 우리는 잘 먹는 것을 좋아합니다.'
        },
        {
          name:'W:',
          speech:'그랜드 투어에 있는 모든 식당들이 그들의 요리로 유명하다는 것을 알면 여러분은 기뻐할 거예요. 언제 어디서, 어디서, 심지어 당신의 방에서도 식사를 할 수 있습니다. 추가 요금 없이.'
        },
        {
          name:'T:',
          speech:'팁을 주는 건 어때요? 서비스도 포함되어 있나요?'
        },
        {
          name:'W:',
          speech:'팁을 주는 것에 대해 걱정할 필요는 없어요. 투어 매니저는 모든 웨이터, 운전사, 가이드에게 돈을 지불합니다.'
        },
        {
          name:'T:',
          speech:'투어 매니저가 통역해 줄 수 있나요? 우리는 외국어를 전혀 하지 않습니다'
        },
        {
          name:'W:',
          speech:'모든 투어 매니저들은 여러 언어를 구사합니다. 그들은 여러분이 필요한 모든 것을 도와줄 수 있습니다.'
        },
        {
          name:'T:',
          speech:'멋지네요.'
        },
        {
          name:'W:',
          speech:'지금 예약해 드릴까요?'
        },
        {
          name:'T:',
          speech:'네. 보증금을 원하세요?'
        },
        {
          name:'W:',
          speech:'네, 감사합니다. 500달러입니다. 저는 당신이 즐거운 여행을 할 것이라는 것을 알아요.'
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
  border-color: transparent #204051 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background: #204051;
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
