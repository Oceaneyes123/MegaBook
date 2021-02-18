<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/driver-with-sunglasses-holding-steering-wheel_23-2148181520.jpg" class="cover-photo">

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
        padding-bottom: 10px;">On the road
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">On the road</li><br />

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
            Do you have a car? (If not, you parents/friend)
          </li>
          <li>
            Have you ever gotten a parking ticket? How about a ticket for speeding?
          </li>
          <li>
            What’s the fastest speed you’ve ever driven
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
                      You were speeding : 당신은 과속하고 있었다<br />                
                    </li>
                    <li>
                      We've been following you : 우리는 당신을 따라가고 있었다
                    </li>
                    <li>
                      break down : 망그러지다, 고장나다
                    </li>
                    <li>
                      send out : 파견하다, 보내다
                    </li>
                    <li>
                      She'll be there in about fifteen minutes : 그녀는 약 15분 안에 그 곳에 있을 것이다
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
          name:'Anne:',
          speech:'Lee! You can’t park here. There’s a fire hydrant.'
        },
        {
          name:'Lee:',
          speech:'Oh, we’ll be back in a few minutes. It’s OK'
        },
        {
          name:'Anne:',
          speech:'Oh, no, it isn’t. You’ll get a parking ticket if you leave it here.'
        },
        {
          name:'Lee:',
          speech:'No, I won’t. It’s five-thirty. All the traffic cops have gone home.'
        },
        {
          name:'Anne:',
          speech:'Oh, Lee....'
        },
        {
          name:'Lee:',
          speech:'Yes?'
        },
        {
          name:'Traffic Officer:',
          speech:'Is this your car, buddy?'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Patrol Officer:',
          speech:'May I see your license?'
        },
        {
          name:'Lee:',
          speech:'Sure.... Oh, I left it at home.'
        },
        {
          name:'Patrol Officer:',
          speech:'In that case, you’ll have to come with us to the station.'
        },
        {
          name:'Lee:',
          speech:'But ... but why?'
        },
        {
          name:'Patrol Officer:',
          speech:'You were speeding, buddy.'
        },
        {
          name:'Lee:',
          speech:'But I was only doing thirty-five!'
        },
        {
          name:'Patrol Officer:',
          speech:'There’s a thirty-mile-an-hour speed limit. It’s a residential section.'
        },
        {
          name:'Lee:',
          speech:'Really? I didn’t see the sign.'
        },
        {
          name:'Patrol Officer:',
          speech:'We’ve been following you.'
        },
        {
          name:'Lee:',
          speech:'So you were doing thirty-five too.'
        },
        {
          name:'Partol Officer:',
          speech:'No. We were doing sixty miles an hour — and we couldn’t catch you!'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Woman',
          speech:'Hello. Turnpike Service Station.'
        },
        {
          name:'Lee:',
          speech:'Hi. I don’t know if you can help me. My car’s broken down.'
        },
        {
          name:'Woman:',
          speech:'We have 24-hour service. Where are you?'
        },
        {
          name:'Lee:',
          speech:'I’m on US 31, just south of Hopeville. My car’s just past the Lone Star Café. It’s a blue Chrysler.'
        },
        {
          name:'Woman:',
          speech:'Do you know what’s wrong with it?'
        },
        {
          name:'Lee:',
          speech:'I have no idea. But it won’t start.'
        },
        {
          name:'Woman:',
          speech:'I’ll send a mechanic out to you. She’ll be there in about fifteen minutes.'
        },
        ],

        translations:[
        {
          name:'Anne:',
          speech:'Lee! 여기 주차하시면 안 돼요. 소화전이 있어요.'
        },
        {
          name:'Lee:',
          speech:'아, 몇 분 후에 돌아올게요. 괜찮아요'
        },
        {
          name:'Anne:',
          speech:'오, 아뇨, 그렇지 않아요. 여기에 주차위반 딱지를 떼시면 됩니다.'
        },
        {
          name:'Lee:',
          speech:'아니요, 안 그럴 거예요. 5시 30분이에요. 교통경찰은 모두 집으로 돌아갔습니다.'
        },
        {
          name:'Anne:',
          speech:'아, Lee.........'
        },
        {
          name:'Lee:',
          speech:'네?'
        },
        {
          name:'교통 담당자:',
          speech:'이게 당신 차예요?'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'순찰 경관:',
          speech:'면허증 좀 보여 주시겠어요?'
        },
        {
          name:'Lee:',
          speech:'그럼요... 아, 집에 두고 왔어요.'
        },
        {
          name:'순찰 경관:',
          speech:'그럴 경우에는 저희와 함께 역까지 가셔야 합니다.'
        },
        {
          name:'Lee:',
          speech:'하지만 왜요?'
        },
        {
          name:'순찰 경관:',
          speech:'속도위반했잖아요, 친구.'
        },
        {
          name:'Lee:',
          speech:'하지만 저는 겨우 35마일로 달리고 있었어요!'
        },
        {
          name:'순찰 경관:',
          speech:'시속 30마일의 속도 제한이 있습니다. 주택가 구간입니다'
        },
        {
          name:'Lee:',
          speech:'정말요? 표지판을 못 봤어요.'
        },
        {
          name:'순찰 경관:',
          speech:'계속 따라다녔어요.'
        },
        {
          name:'Lee:',
          speech:'그럼 당신도  35마일로 달리고 있었군요.'
        },
        {
          name:'순찰 경관:',
          speech:'아니요. 시속 60마일로 달리고 있었는데, 당신을 잡을 수가 없었어요!'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Woman',
          speech:'안녕하세요. 턴파이크 역입니다.'
        },
        {
          name:'Lee:',
          speech:'안녕하세요. 당신이 나를 도와줄 수 있을지 모르겠어요. 제 차가 고장 났어요.'
        },
        {
          name:'Woman:',
          speech:'24시간 서비스가 있어요. 어디 있어요?'
        },
        {
          name:'Lee:',
          speech:'저는 호프빌 바로 남쪽에 있는 미국 31번지에 있어요. 제 차가 론스타 카페를 막 지나갔어요. 블루 크라이슬러입니다.'
        },
        {
          name:'Woman:',
          speech:'뭐가 문제인지 알아요?'
        },
        {
          name:'Lee:',
          speech:'전혀 모르겠어요. 하지만 출발은 안 할 거예요.'
        },
        {
          name:'Woman:',
          speech:'정비사를 보내드릴게요. 그녀는 15분 정도 후에 그곳에 도착할 거예요.'
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
