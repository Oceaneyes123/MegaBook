<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/cheerful-confident-young-female-hotel-receptionist-talking-mobile-phone_23-2148033352.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Making telephone calls
        </h1>

  </v-layout>
  </v-img>

  <div style=" border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border" >Today's topic</h3>
  <div style = "padding : 16px;">

          <p>
            Call 1<br />
          </p>
          <br />
          <table style = "border-collapse: collapse;">

            <tr v-for="call1dialog in call1dialogs" :key="call1dialog">
              <td class = "uppertable" >{{call1dialog.name}}</td>
              <td class = "lowertable" >{{call1dialog.speech}}</td>
            </tr>

          </table>
          <br />
          <p>
            Call 2<br />
          </p>
          <br />
          <table style = "border-collapse: collapse;">

            <tr v-for="call2dialog in call2dialogs" :key="call2dialog">
              <td class = "uppertable" >{{call2dialog.name}}</td>
              <td class = "lowertable" >{{call2dialog.speech}}</td>
            </tr>

          </table>
          <br />
          <p>
            Call 3<br />
          </p>
          <br /><table style = "border-collapse: collapse;">

            <tr v-for="call3dialog in call3dialogs" :key="call3dialog">
              <td class = "uppertable" >{{call3dialog.name}}</td>
              <td class = "lowertable" >{{call3dialog.speech}}</td>
            </tr>

          </table>

  <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
      <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Translation</h3>
        <div style="padding : 16px;">

          <p>
            통화1
          </p>
          <br />
            <table style = "border-collapse: collapse;">

             <tr v-for="call1translation in call1translations" :key="call1translation">
                <td class = "uppertable" >{{call1translation.name}}</td>
                <td class = "lowertable" >{{call1translation.speech}}</td>
              </tr>

            </table>
          <br />
          <p>
            통화 2
          </p>
          <br />
            <table style = "border-collapse: collapse;">

              <tr v-for="call2translation in call2translations" :key="call2translation">
                <td class = "uppertable" >{{call2translation.name}}</td>
                <td class = "lowertable" >{{call2translation.speech}}</td>
              </tr>

            </table>
          <br />
          <p>
            통화 3 
          </p>
          <br />
            <table style = "border-collapse: collapse;">

              <tr v-for="call3translation in call3translations" :key="call3translation">
                 <td class = "uppertable" >{{call3translation.name}}</td>
                <td class = "lowertable" >{{call3translation.speech}}</td>
              </tr>

            </table>
        </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Exercise</h3>
    <div style="padding : 16px;">

      <p>
        Fill in the gaps in the telephone conversation.
      </p>

      <p>
        A: Could I ( &emsp; &emsp; ) to Nathalie, please?<br />
        B: Who's ( &emsp; &emsp; &emsp; &emsp; ),please?<br />
        A: ( &emsp; &emsp; )'s Jessica Keen.<br />
        B: Just a ( &emsp; &emsp; &emsp; &emsp; ),please. Would you like to ( &emsp; &emsp; )?<br />
        A: Yes, please.1<br />
        B: Sorry. I'm ( &emsp; &emsp; ) she's not in her office.<br />
        A: OK, I'll call her ( &emsp; &emsp; ) later.<br />
      </p>
      <p>
        Free response:<br />
        Do you or your colleagues speak English on the telephone? Who do you speak to?
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
                    <b>will:</b> spontaneous decisions and offers
                  </p>
                  <p>
                    <b>I'll</b> give her the message.<br />
                    <b>She'll</b> call you back.<br />
                    (I'll=I will)
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
        call1dialogs:[
        {
          name:'Reception:',
          speech:'Hello. Camden Marketing.'
        },
        {
          name:'Rob:',
          speech:'Hello. Could I speak to Louise Miller, please?'
        },
        {
          name:'Reception:',
          speech:'Who’s calling, please?'
        },
        {
          name:'Rob:',
          speech:'Rob Sears.'
        },
        {
          name:'Reception:',
          speech:'Her line’s busy at the moment.'
        },
        {
          name:'Rob:',
          speech:'Oh, right. Um... OK. I’ll call back later.'
        },
        {
          name:'Reception:',
          speech:'OK.'
        },
        {
          name:'Rob:',
          speech:'Bye.'
        },
        {
          name:'Reception:',
          speech:'Bye.'
        },
        ],

        call2dialogs:[
        {
          name:'Reception:',
          speech:'Hello. Camden Marketing.'
        },
        {
          name:'Rob:',
          speech:'Hello. Louise Miller, please. It’s Rob Sears.'
        },
        {
          name:'Reception:',
          speech:'One moment, please. I’m afraid she’s still on the phone. Would you like to hold?'
        },
        {
          name:'Rob:',
          speech:'Um... Could you ask her to call me back?'
        },
        {
          name:'Reception:',
          speech:'Yes.'
        },
        {
          name:'Rob:',
          speech:'She has my number.'
        },
        {
          name:'Reception:',
          speech:'Could I take your name again?'
        },
        {
          name:'Rob:',
          speech:'Yeah. Rob Sears. S-E-A-R-S.'
        },
        {
          name:'Reception:',
          speech:'OK. I’ll give her the message as soon as possible.'
        },
        {
          name:'Rob:',
          speech:'OK. Thanks very much. Bye.'
        },
        {
          name:'Reception:',
          speech:'Bye.'
        },
        ],

        call3dialogs:[
        {
          name:'Rob:',
          speech:'Hello.'
        },
        {
          name:'Louise:',
          speech:'Hello. Is that Rob?'
        },
        {
          name:'Rob:',
          speech:'Yes, speaking.'
        },
        {
          name:'Louise:',
          speech:'Hi, Rob. It’s Louise.'
        },
        {
          name:'Rob:',
          speech:'Oh hi, Louise. Thanks for calling back.'
        },
        {
          name:'Louise:',
          speech:'You’re welcome. What can I do for you?'
        },  
        ],

        
        call1translations:[
        {
          name:'수신:',
          speech:'여보세요. 캠든 마케팅입니다.'
        },
        {
          name:'롭:',
          speech:'여보세요. 루이즈 밀러와 통화할 수 있을까요?'
        },
        {
          name:'수신:',
          speech:'누구시죠?'
        },
        {
          name:'롭:',
          speech:'롭 시어스입니다.'
        },
        {
          name:'수신:',
          speech:'그녀는 지금 통화중입니다.'
        },
        {
          name:'롭:',
          speech:'아, 그렇군요. 음... 알았어요. 나중에 다시 전화할게요.'
        },
        {
          name:'수신:',
          speech:'네.'
        },
        {
          name:'롭:',
          speech:'안녕히계세요.'
        },
        {
          name:'수신:',
          speech:'안녕히계세요.'
        },
        ],

        call2translations:[
        {
          name:'수신:',
          speech:'여보세요. 캠든 마케팅입니다.'
        },
        {
          name:'롭:',
          speech:'여보세요. 루이즈 밀러 부탁드려요. 롭 시어스입니다.'
        },
        {
          name:'수신:',
          speech:'잠깐만요. 유감스럽게도 그녀는 아직 통화 중입니다. 기다리시겠습니까?'
        },
        {
          name:'롭:',
          speech:'음... 그녀에게 다시 전화해 달라고 전해 주시겠습니까?'
        },
        {
          name:'수신:',
          speech:'네.'
        },
        {
          name:'롭:',
          speech:'그녀는 내 전화번호를 알고 있습니다.'
        },
        {
          name:'수신:',
          speech:'성함이 어떻게 되시죠?'
        },
        {
          name:'롭:',
          speech:'네. 롭 시어스, S-E-A-R-S'
        },
        {
          name:'수신:',
          speech:'네. 나는 가능한 한 빨리 그녀에게 메시지를 전하겠습니다.'
        },
        {
          name:'롭:',
          speech:'알겠습니다. 정말 고마워요. 안녕히 계세요.'
        },
        {
          name:'수신:',
          speech:'안녕히 계세요.'
        },
        ],

        call3translations:[
        {
          name:'롭:',
          speech:'Hello.'
        },
        {
          name:'루이즈:',
          speech:'Hello. Is that Rob?'
        },
        {
          name:'롭:',
          speech:'Yes, speaking.'
        },
        {
          name:'루이즈:',
          speech:'Hi, Rob. It’s Louise.'
        },
        {
          name:'롭:',
          speech:'Oh hi, Louise. Thanks for calling back.'
        },
        {
          name:'루이즈:',
          speech:'You’re welcome. What can I do for you?'
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
