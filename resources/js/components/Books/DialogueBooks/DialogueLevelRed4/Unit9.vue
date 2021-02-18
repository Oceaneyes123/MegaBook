<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://cdn.pixabay.com/photo/2016/09/17/07/31/blue-light-1675687_960_720.jpg" class="cover-photo">

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
        padding-bottom: 10px;">An interrogation
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">An interrogation</li><br />

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
          <u>Ask questions</u><br />
          Ex) You are my English teacher, aren’t you?<br />
        </p>
        <br />

        <ol style="margin: 12px;">
          <li>
            This lesson is fun, <u> &emsp; &emsp; &emsp; </u>? <br />
          </li>
          <li>
            I am not making many mistakes, <u> &emsp; &emsp; &emsp; </u>? <br />
          </li>
          <li>
            You’re a good teacher, <u> &emsp; &emsp; &emsp; </u>? <br />
          </li>
          <li>
            You live in the Philippines, <u> &emsp; &emsp; &emsp; </u>? <br />
          </li>
          <li>
            Yesterday, it rained a lot in the Philippines, <u> &emsp; &emsp; &emsp; </u>? <br />
          </li>
          <li>
            I speak English very well, <u> &emsp; &emsp; &emsp; </u>? <br />
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
          뉴욕 시내 금융가에서 은행 강도가 들었어요. 경찰은 오후 6시에 Staten Island에 있는 그의 아파트에서 한 남자를 체포했습니다. 한 형사가 지금 그를 심문하고 있습니다.<br />
        </p>
        <br />
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
                      부가의문문 : 상대방의 동의를 구하거나 사실을 확인하기 위해 평서문 끝에 짧게 붙이는 의문문입니다.<br />
                          - 조동사 + 주어의 형태이며 그렇지? 그렇지 않니?라고 해석합니다.<br />
                          - 긍정문 뒤에는 부정으로, 부정문 뒤에는 긍정으로 만들고 앞 문장의 주어가 명사이면 대명사로 바꿔 씁니다.<br />
                          - 앞 문장에 be동사와 조동사가 있으면 그대로 사용하고, 일반동사가 있으면 주어의 인칭과 수,일반동사의 시제에 따라 do, does, did를 사용합니다.<br />
                    </li>
                    <li>
                      get to ~ in time : 시간 안에 ~에 도착하다.<br />
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
          name:'Police Detective:',
          speech:'You’re John Patrick O’Brien, aren’t you?'
        },
        {
          name:'O’Brien:',
          speech:'Yes, I am.'
        },
        {
          name:'PD:',
          speech:'You went to the races at Montvale yesterday, didn’t you?'
        },
        {
          name:'O’B:',
          speech:'That’s right.'
        },
        {
          name:'PD:',
          speech:'You weren’t alone, were you?'
        },
        {
          name:'O’B:',
          speech:'No, I wasn’t. I was with my friend, Bobbie Ann Chase.'
        },
        {
          name:'PD:',
          speech:'You left your apartment at eleven o’clock, didn’t you?'
        },
        {
          name:'O’B:',
          speech:'Yes. About eleven.'
        },
        {
          name:'PD:',
          speech:'You had lunch at a Chinese restaurant, didn’t you?'
        },
        {
          name:'O’B:',
          speech:'No, we didn’t. We had lunch at a fast food place.'
        },
        {
          name:'PD:',
          speech:'You don’t remember the name of the place, do you?'
        },
        {
          name:'O’B:',
          speech:'No, I’m afraid I don’t.'
        },
        {
          name:'PD:',
          speech:'You got to Montvale racetrack in time for the first race, didn’t you?'
        },
        {
          name:'O’B:',
          speech:'Yes, correct.'
        },
        {
          name:'PD:',
          speech:'You said you stayed there until the last race at 5 o’clock, didn’t you?'
        },
        {
          name:'O’B:',
          speech:'That’s correct.'
        },
        {
          name:'PD:',
          speech:'You won $50,000, didn’t you?'
        },
        {
          name:'O’B:',
          speech:'I can’t remember exactly how much.'
        },
        {
          name:'PD:',
          speech:'There was $50,000 in your apartment, wasn’t there?'
        },
        {
          name:'O’B:',
          speech:'Was there?'
        },
        {
          name:'PD:',
          speech:'You don’t know where Bobbie Ann is now, do you?'
        },
        {
          name:'O’B:',
          speech:'No, I’m not her husband, am I?'
        },
        {
          name:'PD:',
          speech:'It’s interesting, isn’t it, O’Brien? You have a very fast car, don’t you?'
        },
        {
          name:'O’B:',
          speech:'What do you mean?'
        },
        {
          name:'PD:',
          speech:'The last race at Montvale started late, and it didn’t finish until twenty-five after five, so you drove from Montvale on' +
                  ' Long Island to midtown Manhattan to Staten Island in 35 minutes — at rush hour! That’s impossible, isn’t it, O’Brien?'
        },
        ],

        translations:[
        {
          name:'경찰 형사입니다:',
          speech:'John Patrick O’Brien 맞죠?'
        },
        {
          name:'O’Brien:',
          speech:'네, 그렇습니다.'
        },
        {
          name:'PD:',
          speech:'어제 Montvale  경주에 갔죠?'
        },
        {
          name:'O’B:',
          speech:'맞습니다.'
        },
        {
          name:'PD:',
          speech:'혼자는 아니었죠?'
        },
        {
          name:'O’B:',
          speech:'아뇨, 그렇지 않았어요. 저는 제 친구 Bobbie Ann Chase와 함께 있었어요.'
        },
        {
          name:'PD:',
          speech:'열한 시에 아파트를 나왔죠?'
        },
        {
          name:'O’B:',
          speech:'네. 11시쯤에요.'
        },
        {
          name:'PD:',
          speech:'중식당에서 점심을 먹었죠?'
        },
        {
          name:'O’B:',
          speech:'아뇨, 안 그랬어요. 우리는 패스트푸드점에서 점심을 먹었어요.'
        },
        {
          name:'PD:',
          speech:'지명 기억 안 나죠?'
        },
        {
          name:'O’B:',
          speech:'아니요, 저는 그렇게 생각하지 않습니다.'
        },
        {
          name:'PD:',
          speech:'첫 경주에 맞춰 Montvale 경마장에 도착했죠?'
        },
        {
          name:'O’B:',
          speech:'네, 맞습니다.'
        },
        {
          name:'PD:',
          speech:'5시에 마지막 경주 때까지 거기 있었다고 했죠?'
        },
        {
          name:'O’B:',
          speech:'맞습니다.'
        },
        {
          name:'PD:',
          speech:'5만 달러 땄죠?'
        },
        {
          name:'O’B:',
          speech:'정확히 얼마인지 기억이 안 나요.'
        },
        {
          name:'PD:',
          speech:'당신 아파트에는 5만 달러가 있었죠?'
        },
        {
          name:'O’B:',
          speech:'있었어요?'
        },
        {
          name:'PD:',
          speech:'Bobbie Ann이 지금 어디 있는지 모르죠?'
        },
        {
          name:'O’B:',
          speech:'아뇨, 전 그녀의 남편이 아닙니다. 그렇죠?'
        },
        {
          name:'PD:',
          speech:'흥미롭죠, O’Brien? 당신은 매우 빠른 차를 가지고 있군요, 그렇죠?'
        },
        {
          name:'O’B:',
          speech:'무슨 뜻이에요?'
        },
        {
          name:'PD:',
          speech:'Montvale 에서의 마지막 경주는 늦게 시작되었고, 5시 25분이 지나서야 끝이 났기 때문에 Montvale 에서 차를 타고 온 거죠.' +
                  ' 롱아일랜드에서 맨해튼 미드타운까지 35분 뒤면 스태튼아일랜드까지 출퇴근 시간에 도착합니다! 그건 불가능하죠, O’Brien?'
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
