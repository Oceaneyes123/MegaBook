<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/female-receptionist-working-front-desk_53876-20945.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Reservations
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Reservations</li><br />

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
            What do you think about the behavior of the band members?
          </li>
          <li>
            Did the manager accept the reservation or not?
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
                      please hold : 끊지 말고 기다리세요 <br />                 
                    </li>
                    <li>
                      put through : ~의 전화를 연결시키다
                    </li>
                    <li>
                      "I'm afraid I cannot accept your reservation" : 당신의 예약을 받아드릴 수 없을 것 같습니다
                    </li>
                    <li>
                      stay at : ~에 머무르다
                    </li>
                      pay an account (셈을 끝내다) (You haven't paid the account for the last time yet : 당신은 지난번 결제도 아직 안했습니다)
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
          name:'Operator:',
          speech:'Glory Inn, Atlanta. How can I help you?'
        },
        {
          name:'Zoot:',
          speech:'Hi, this is Zoot Lambert. The manager of Titanium? You know, the band.... I want...'
        },
        {
          name:'Operator:',
          speech:'Please hold, Mr. Lambert. I’m putting you through to the reservations manager.'
        },
        {
          name:' ',
          speech:'  '
        },
        {
          name:'Manager:',
          speech:'Mr. Lambert? This is Lauren Perry, the hotel manager'
        },
        {
          name:'Zoot:',
          speech:'Oh, yeah? Well, I need five rooms for Friday night. That’s the 15th. I want the best rooms in the hotel.'
        },
        {
          name:'Manager:',
          speech:'Sorry, I’m afraid I cannot accept your reservation'
        },
        {
          name:'Zoot:',
          speech:'Now look, we always stay at the Glory Inn...'
        },
        {
          name:'Manager:',
          speech:'I know that, sir. Last time you were here, we had a number of complaints from other guests.'
        },
        {
          name:'Zoot:',
          speech:'You mean they don’t like long-haired rock musicians!'
        },
        {
          name:'Manager:',
          speech:'That’s not the problem, sir. The band used bad language in the coffee shop, and threw two TV sets into the pool.'
        },
        {
          name:'Zoot:',
          speech:'Yeah, yeah. Well, they’ll be more careful this time.'
        },
        {
          name:'Manager:',
          speech:'I’m afraid that’s not all, sir. You haven’t paid the account for the last time yet.'
        },
        {
          name:'Zoot:',
          speech:'I’ll put a check in the mail.'
        },
        {
          name:'Manager:',
          speech:'Please do.'
        },
        {
          name:'Zoot:',
          speech:'So, what about our reservation for Friday?'
        },
        ],

        translations:[
        {
          name:'운영자:',
          speech:'애틀랜타의 글로리 인입니다. 무엇을 도와드릴까요?'
        },
        {
          name:'Zoot:',
          speech:'안녕하세요, Zoot Lambert입니다. Titanium매니저요? 있잖아요, 밴드가... 저는...'
        },
        {
          name:'운영자:',
          speech:'잠시만 기다려 주세요, Lambert 씨. 예약 담당자와 연결해 드리겠습니다.'
        },
        {
          name:' ',
          speech:'  '
        },
        {
          name:'매니저:',
          speech:'램버트 씨요? 호텔 매니저 Lauren Perry입니다.'
        },
        {
          name:'Zoot:',
          speech:'아, 그래요? 금요일 밤에 묵을 방이 다섯 개 필요해요. 그게 15일입니다. 저는 그 호텔에서 가장 좋은 방을 원합니다..'
        },
        {
          name:'매니저:',
          speech:'죄송합니다, 죄송하지만, 예약을 수락할 수 없습니다.'
        },
        {
          name:'Zoot:',
          speech:'자, 보세요, 우리는 항상 글로리 인에 머무릅니다.'
        },
        {
          name:'매니저:',
          speech:'다음을 수행합니다. 저도 알아요, 선생님. 지난번 당신이 여기 왔을 때, 우리는 다른 손님들로부터 많은 불평을 들었습니다.'
        },
        {
          name:'Zoot:',
          speech:'그들이 긴 머리의 록 뮤지션들을 좋아하지 않는다는 뜻인가요!'
        },
        {
          name:'매니저:',
          speech:'그게 문제가 아닙니다. 그 밴드는 커피숍에서 욕을 했고, 두 대의 TV를 수영장에 던졌습니다.'
        },
        {
          name:'Zoot:',
          speech:'네, 그래요. 음, 이번에는 좀 더 조심할 거예요.'
        },
        {
          name:'매니저:',
          speech:'유감스럽게도 그게 다가 아닙니다. 당신은 아직 마지막으로 돈을 지불하지 않았습니다.'
        },
        {
          name:'Zoot:',
          speech:'수표를 우편으로 부치겠습니다.'
        },
        {
          name:'매니저:',
          speech:'그렇게 해주세요.'
        },
        {
          name:'Zoot:',
          speech:'그럼, 금요일로 예약하면 어떨까요?'
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
