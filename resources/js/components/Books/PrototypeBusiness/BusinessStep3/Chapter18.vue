<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGyH6cBB0/4/screen_2x/canva-orange-and-green-label-airplane-ticket-MADGyH6cBB0.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Confirming arrangements
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
            Where does he want to go?
          </li>
          <li>
            What type of ticket does he want?
          </li>
          <li>
            What item of luggage does he want to take?
          </li>
          <li>
            Complete the information : Date of departure:<br />
            &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &nbsp; &thinsp; Date of return trip:<br />
            &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &nbsp; &thinsp; Price of ticket:<br />
            &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &nbsp; &thinsp; Baggage allowance:<br />
            &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &nbsp; &thinsp; Excess baggage charge:
          </li>
        </ol>

        <p>
          Free response:<br />
          Discuss air travel.<br />
          Which airlines do you use?<br />
          Which is your favorite airline?<br />
          Do you often fly long distances?<br />
          Do you like travelling by plane? Why/Why not?
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
                Useful language<br />
                I’d like to book flight to Barcelona.<br />
                If you book two months in advance there’s a 10% discount.<br />
                Are there any extra charges or is everything included in the fare?<br />
                If I cancel the booking can I get refund?<br />
                If you go over the baggage allowance, the excess baggage charge is ten pounds per kg.
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
          name:'Assistant:',
          speech:'GlenAir, good afternoon. How can I help you?'
        },
        {
          name:'Customer:',
          speech:'Hello. I’d like to fly to Lisbon at the end of May.'
        },
        {
          name:'Assistant:',
          speech:'Lisbon?'
        },
        {
          name:'Customer:',
          speech:'Yes.'
        },{
          name:'Assistant:',
          speech:'What date are you planning to leave?'
        },
        {
          name:'Customer:',
          speech:'On May the twenty-fourth.'
        },
        {
          name:'Assistant:',
          speech:'May the twenty-fourth. Is it a return flight?'
        },
        {
          name:'Customer:',
          speech:'A return, yes. I want to come back on the thirty-first.'
        },
        {
          name:'Assistant:',
          speech:'The thirty-first of May… OK, the cheapest fare’s fifty-five pounds.'
        },
        {
          name:'Customer:',
          speech:'That’s for a return.'
        },
        {
          name:'Assistant:',
          speech:'Yes.'
        },
        {
          name:'Customer:',
          speech:'OK. Um… and can I change the date if I need to?'
        },
        {
          name:'Assistant:',
          speech:'No. For that fare, you can’t change the booking, and there’s no refund if you cancel.'
        },
        {
          name:'Customer:',
          speech:'Right. So fifty-five pounds. And are there any extra charges? For airport tax, or…'
        },
        {
          name:'Assistant:',
          speech:'No, that’s included.'
        },
        {
          name:'Customer:',
          speech:'OK. Um… oh, that’s the other question-what’s the maximum baggage allowance? Because I want to take a surfboard with me.'
        },
        {
          name:'Assistant:',
          speech:'Right. Well, the maximum allowance is twenty kilograms. The excess baggage charge is six pounds per kilogram, but for a surfboard…'
        },
        ],

        translations:[
        {
          name:'보조자:',
          speech:'글렌에어, 좋은 오후입니다. 제가 무엇을 도와드릴까요?'
        },
        {
          name:'고객:',
          speech:'안녕하세요. 5월 말에 리스본에 가고 싶은데.'
        },
        {
          name:'보조자:',
          speech:'리스본이요?'
        },
        {
          name:'고객:',
          speech:'네.'
        },{
          name:'보조자:',
          speech:'언제 떠날 예정이신가요?'
        },
        {
          name:'고객:',
          speech:'5월 24일이요.'
        },
        {
          name:'보조자:',
          speech:'24일 5월 24일. 왕복 비행기인가요?'
        },
        {
          name:'고객:',
          speech:'왕복, 맞습니다. 저는 31일에 다시 오고 싶습니다.'
        },
        {
          name:'보조자:',
          speech:'5월 31일... 알겠습니다, 가장 싼 요금은 55파운드입니다.'
        },
        {
          name:'고객:',
          speech:'그건 왕복이죠.'
        },
        {
          name:'보조자:',
          speech:'네.'
        },
        {
          name:'고객:',
          speech:'네. 음… 그리고 필요하다면 날짜를 변경해도 될까요?'
        },
        {
          name:'보조자:',
          speech:'아니요. 그 요금은 예약을 변경할 수 없고, 취소하면 환불이 안 됩니다.'
        },
        {
          name:'고객:',
          speech:'그렇군요, 그래서 55파운드군요. 그리고 추가요금은 없습니까? 공항세, 또는…'
        },
        {
          name:'보조자:',
          speech:'아니요, 그것은 포함되어 있습니다.'
        },
        {
          name:'고객:',
          speech:'네. 음, 다른 질문인데, 최대 수하물 허용 한도는 얼마입니까? 왜냐하면 서프보드와 같이 타고 싶기 때문입니다.'
        },
        {
          name:'보조자:',
          speech:'그렇군요. 글쎄요, 최대 허용량은 20kg입니다. 초과 수화물 요금은 1kg당 6파운드지만, 서핑 보드는…'
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
