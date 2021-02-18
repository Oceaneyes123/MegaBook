<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGx7HePZE/4/screen_2x/canva-train-station-MADGx7HePZE.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 class="upper-header-BS2">Buying train tickets
      </h1>
    </v-layout>
  </v-img>

  <div class="top-line-BS2">
  </div>
  <h3  class = "lower-header-BS2" >Today's topic</h3>
  <div style = "padding : 16px;">

   
<table style = "border-collapse: collapse;">

  <tr v-for="dialog in dialogs" :key="dialog">
    <td class = "uppertable" >{{dialog.name}}</td>
    <td class = "lowertable" >{{dialog.speech}}</td>
  </tr>

</table>



   <div class = "line-BS2">
   </div>
   <h3 class = "border-BS2">Translation</h3>
   <div style="padding : 16px;">
    
    <table style = "border-collapse: collapse;">

      <tr v-for="translation in translations" :key="translation">
        <td class = "uppertable" >{{translation.name}}</td>
        <td class = "lowertable" >{{translation.speech}}</td>
      </tr>

    </table>
   </div>



      <div class = "line-BS2">
      </div>
      <h3 class = "border-BS2">Exercise</h3>
      <div style="padding : 16px;">

        <p>
          Complete the questions to match the answers.
        </p>

        <ol style="margin: 12px;">
          <li>
            A: ( &emsp; &emsp; ) would you like to go?<br />
            B: I'd like to go to Milan.
          </li>
          <li>
             A: ( &emsp; &emsp; ) do you want to pay?<br />
             B: I want to pay by credit card.
          </li>
          <li>
            A: ( &emsp; &emsp; ) you like a single or a return?<br />
            B: I'd like a single, please.
          </li>
          <li>
             A: ( &emsp; &emsp; ) do you want to come back?<br />
             B: I want to come back on Monday.
          </li>
          <li>
             A: ( &emsp; &emsp; ) you like to book a seat now?<br />
             B: Yes, I'd like to book a seat now.
          </li>
          <li>
             A: ( &emsp; &emsp; ) you want to travel second class?<br />
             B: No, I want to travel first class, please.
          </li>
        </ol>

        <p>
          Free response:<br />
          How often do you travel by train?<br />
          Do you like train travel?<br />
          Do you usually reserve a seat?
        </p>

      </div>

      <div class = "line-BS2">
      </div>
      <h3 class = "border-BS2">Self Study</h3>
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
                      want to + 부정사 / would like to + 부정사
                    </p>
                    <p>
                      I'd like to book a seat.<br />
                      I want to book a seat.
                    </p>
                    <p>
                      When would you like to leave?<br />
                      When do you want to leave?
                    </p>
                    <p>
                      When do you want to leave?
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
          speech:'Hello.'
        },
        {
          name:'Gary:',
          speech:'Hi. I’d like to book two seats to Paris, please. For tomorrow.'
        },
        {
          name:'Assistant:',
          speech:'At what time?'
        },
        {
          name:'Gary:',
          speech:'At about 5.00 pm. I don’t have a timetable.'
        },
        {
          name:'Assistant:',
          speech:'There’s a train at 17.15. It arrives in Paris at 20.55, local time.'
        },
        {
          name:'Gary:',
          speech:'Right. OK, that’s fine.'
        },
        {
          name:'Assistant:',
          speech:'Would you like to travel first class or standard class?'
        },
        {
          name:'Gary:',
          speech:'Standard.'
        },
        {
          name:'Assistant:',
          speech:'And would you like a single or a return ticket?'
        },
        {
          name:'Gary:',
          speech:'A round-trip, please.'
        },
        {
          name:'Assistant:',
          speech:'When would you like to come back?'
        },
        {
          name:'Gary:',
          speech:'I want to return on Saturday, but I don’t know what time.'
        },
        {
          name:'Assistant:',
          speech:'Do you want to book the return trip now?'
        },
        {
          name:'Gary:',
          speech:'If I reserve a seat, Can I change the reservation?'
        },
        {
          name:'Assistant:',
          speech:'With a standard fare, you can change or cancel the booking, yes.'
        },
        {
          name:'Gary:',
          speech:'OK. How much is the standard fare, then?'
        },
        {
          name:'Assistant:',
          speech:'One moment.'
        },
        ],

        translations:[
        {
          name:'보조자:',
          speech:'안녕하세요.'
        },
        {
          name:'개리:',
          speech:'안녕하세요. 파리행 좌석 두 개를 예약하고 싶어요. 내일거로.'
        },
        {
          name:'보조자:',
          speech:'몇 시로 할까요?'
        },
        {
          name:'개리:',
          speech:'오후 5시쯤이요. 저는 시간표가 없어요.'
        },
        {
          name:'보조자:',
          speech:'17시 15분에 기차가 있어요. 그것은 현지시간 20시 55분에 파리에 도착합니다.'
        },
        {
          name:'개리:',
          speech:'R그렇군요. 괜찮습니다.'
        },
        {
          name:'보조자:',
          speech:'일등석으로 하시겠습니까, 일반석으로 하시겠습니까?'
        },
        {
          name:'개리:',
          speech:'일반석이요.'
        },
        {
          name:'보조자:',
          speech:'그리고 편도티켓으로 하시겠습니까, 왕복티켓으로 하시겠습니까?'
        },
        {
          name:'개리:',
          speech:'왕복으로 부탁드려요.'
        },
        {
          name:'보조자:',
          speech:'언제 돌아오시겠습니까?'
        },
        {
          name:'개리:',
          speech:'토요일에 돌아가고 싶은데, 몇 시인지 모르겠어요.'
        },
        {
          name:'보조자:',
          speech:'지금 돌아오는 여행을 예약하시겠습니까?'
        },
        {
          name:'개리:',
          speech:'I만약 내가 좌석을 예약한다면, 예약을 바꿀 수 있을까요?'
        },
        {
          name:'보조자:',
          speech:'표준요금으로 예약을 변경하거나 취소할 수 있습니다.'
        },
        {
          name:'개리:',
          speech:'알았어요. 그럼 표준요금은 얼마지요?'
        },
        {
          name:'보조자:',
          speech:'잠시만요.'
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




</style>
