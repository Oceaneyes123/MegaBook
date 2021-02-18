<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGyf8N3NE/4/screen_2x/canva-person-holding-white-stylus-MADGyf8N3NE.jpg" class = "cover-photo">

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

        <p>
          Complete the information.
        </p>

        <ol style="margin: 12px;">
          <li>
            Date of meeting: <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
          </li>
          <li>
            Time of meeting: <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
          </li>
          <li>
            Document to email: <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
          </li>
        </ol>

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
                Present tenses as future
                </p>
                <p>
                  Future timetables/schedules: present simple<br />
                  The flight lands at 11.00.
                </p>
                <p>
                  Future arrangements: present continuous<br />
                  I’m flying at San Francisco next month.
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
          name:'Naomi:',
          speech:'So, when’s the best time to meet, for you? I’m free next week.'
        },
        {
          name:'Tom:',
          speech:'Um… I can’t make it next week. I’m… I’m busy all week. The week after is OK for me.'
        },
        {
          name:'Naomi:',
          speech:'The week after. What about Monday? Monday, December the twelfth?'
        },
        {
          name:'Tom:',
          speech:'Yes, that’s OK for me.'
        },
        {
          name:'Naomi:',
          speech:'In the morning?'
        },
        {
          name:'Tom:',
          speech:'Yeah.'
        },
        {
          name:'Naomi:',
          speech:'Half past nine?'
        },
        {
          name:'Tom:',
          speech:'Nine thirty? Yeah, that’s fine.'
        },
        {
          name:'Naomi:',
          speech:'OK. Monday, December the twelfth at nine thirty, then.'
        },
        {
          name:'Tom:',
          speech:'And can you send me an agenda?'
        },
        {
          name:'Naomi:',
          speech:'Yes, I’ll write an agenda this morning, and send it to you this afternoon.'
        },
        {
          name:'Tom:',
          speech:'Excellent. OK, so I look forward to receiving that, and I’ll see you on the twelfth.'
        },
        {
          name:'Naomi:',
          speech:'OK. I look forward to seeing you then.'
        },
        {
          name:'Tom:',
          speech:'OK. Bye.'
        },
        {
          name:'Naomi:',
          speech:'Bye.'
        },
        ],

      translations:[
      {
          name:'나오미:',
          speech:'그럼, 언제 만나는 게 가장 좋을까요? 저는 다음 주에 시간이 있어요.'
        },
        {
          name:'톰:',
          speech:'음… 다음 주에는 못 갈 것 같아요. 저는 일주일 내내 바빠요. 저는 그 다음 주가 괜찮아요.'
        },
        {
          name:'나오미:',
          speech:'그 다음 주에요. 월요일은 어때요? 12월 12일 월요일요?'
        },
        {
          name:'톰:',
          speech:'네, 저는 괜찮아요.'
        },
        {
          name:'나오미:',
          speech:'아침에요?'
        },
        {
          name:'톰:',
          speech:'그래요.'
        },
        {
          name:'나오미:',
          speech:'9시 반요?'
        },
        {
          name:'톰:',
          speech:'9시 30분요? 네, 괜찮아요.'
        },
        {
          name:'나오미:',
          speech:'알겠습니다. 그럼 12월 12일 월요일 9시 30분입니다.'
        },
        {
          name:'톰:',
          speech:'그리고 저에게 안건을 보내주실 수 있나요?'
        },
        {
          name:'나오미:',
          speech:'네, 오늘 아침에 안건을 작성해서 오후에 보내드리겠습니다.'
        },
        {
          name:'톰:',
          speech:'좋아요. 네, 잘 부탁드리겠습니다. 12일에 뵙겠습니다.'
        },
        {
          name:'나오미:',
          speech:'알겠습니다. 그때 뵙기를 기대합니다.'
        },
        {
          name:'톰:',
          speech:'아요. 안녕히 계세요.'
        },
        {
          name:'나오미:',
          speech:'안녕히 계세요.'
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
