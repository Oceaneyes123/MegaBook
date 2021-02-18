<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/front-view-young-girl-boy-talking-phones_23-2148465754.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Making arrangements 
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
          Answer the questions.
        </p>

        <ol style="margin: 12px;">
          <li>
            What do Sylvie and Michael decide to do?
          </li>
          <li>
            What does Michael say he’ll do today?
          </li>
          <li>
            What does Sylvie say she’ll do today?
          </li>
          <li>
            When do they arrange to speak again?
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
                <b>Will/shall</b> : offers and suggestions<br />
                Offers: <b>I’ll… Shall…?</b><br />
                We need more information about this.<br />
                <b>I’ll</b> look on the Internet.
                </p>
                <p>
                  We need to book our tickets.<br />
                  <b>Shall I</b> book them?
                </p>
                <p>
                  Suggestions: <b>Shall we…?</b><br />
                  When can we talk?<br />
                  <b>Shall we</b> speak this afternoon?
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
          name:'Michael:',
          speech:'Hello.'
        },
        {
          name:'Sylvie:',
          speech:'Hello. Is that Michael?'
        },
        {
          name:'Michael:',
          speech:'Speaking.'
        },
        {
          name:'Sylvie:',
          speech:'Hi Michael, It’s Sylvie in Brussels.'
        },
        {
          name:'Michael:',
          speech:'Hi Sylvie, how are you?'
        },
        {
          name:'Sylvie:',
          speech:'Fine, thanks. You?'
        },
        {
          name:'Michael:',
          speech:'Yeah, very well, thanks.'
        },
        {
          name:'Sylvie:',
          speech:'Are you getting ready for the conference next month?'
        },
        {
          name:'Michael:',
          speech:'Um… not really. What about you?'
        },
        {
          name:'Sylvie:',
          speech:'Well, that’s what I’m phoning about, actually. How are you going to San Francisco? Are you flying direct from Dublin?'
        },
        {
          name:'Michael:',
          speech:'Um… well, I still need to book my flight. But I’ll probably have to change in… either in London or… in Amsterdam. What about you?'
        },
        {
          name:'Sylvie:',
          speech:'Well, I still need to book my flight, from Amsterdam. So, um…'
        },
        {
          name:'Michael:',
          speech:'Well, shall we catch the same flight?'
        },
        {
          name:'Sylvie:',
          speech:'Yeah, That’s what I thought, actually. Then we can work on the plane.'
        },
        {
          name:'Michael:',
          speech:'Yeah, that makes sense. So I need to book a flight to Amsterdam, then. Shall I look into flights to San Francisco, as well?'
        },
        {
          name:'Sylvie:',
          speech:'Um… yeah, if that’s OK.'
        },
        {
          name:'Michael:',
          speech:'Yeah, no problem. I’ll look on the Internet after lunch and, um… I’ll call you back. What about booking a hotel?'
        },
        {
          name:'Sylvie:',
          speech:'Um… Well, shall I contact the San Francisco office… see if they know any good places? I can get in touch with Rita.'
        },
        {
          name:'Michael:',
          speech:'Yeah, good idea.'
        },
        {
          name:'Sylvie:',
          speech:'I’ll give her a call this afternoon, as soon as the office opens.'
        },
        {
          name:'Michael:',
          speech:'Excellent. So I’ll look into flights. And, um… I’ll get back to you.'
        },
        {
          name:'Sylvie:',
          speech:'Great. Shall we speak at about four thirty?'
        },
        {
          name:'Michael:',
          speech:'Yes, fine. I’ll call you then.'
        },
        {
          name:'Sylvie:',
          speech:'OK. Bye.'
        },
        {
          name:'Michael:',
          speech:'Thanks for calling, Sylvie. Bye.'
        },
        ],

        translations:[
        {
          name:'마이클:',
          speech:'여보세요.'
        },
        {
          name:'실비:',
          speech:'여보세요. 마이클이에요?'
        },
        {
          name:'마이클:',
          speech:'네.'
        },
        {
          name:'실비:',
          speech:'안녕하세요 마이클, 브뤼셀에 있는 실비입니다.'
        },
        {
          name:'마이클:',
          speech:'안녕하세요 실비, 잘 지내세요?'
        },
        {
          name:'실비:',
          speech:'좋아요, 고마워요, 당신은요?'
        },
        {
          name:'마이클:',
          speech:'네 잘지내요, 고마워요.'
        },
        {
          name:'실비:',
          speech:'다음 달에 있을 회의 준비는 다 됐어요?'
        },
        {
          name:'마이클:',
          speech:'음… 별로요. 당신은요?'
        },
        {
          name:'실비:',
          speech:'음, 그게 바로 제가 전화하는 이유입니다. 샌프란시스코에는 어떻게 가실 건가요? 더블린에서 직항하는 건가요?'
        },
        {
          name:'마이클:',
          speech:'음, 아직 비행기 예약을 해야 하거든요. 하지만 런던이나 암스테르담에서 갈아타야 할 것 같아요. 당신은요?'
        },
        {
          name:'실비:',
          speech:'음, 암스테르담에서 출발하는 비행기를 아직 예약해야 해요. 그럼요, 음…'
        },
        {
          name:'마이클:',
          speech:'그럼, 같은 비행기를 탈까요?'
        },
        {
          name:'실비:',
          speech:'네, 사실 저도 그렇게 생각했어요. 그럼 비행기에서 일할 수 있겠네요.'
        },
        {
          name:'마이클:',
          speech:'네, 좋네요. 그럼 암스테르담행 비행기를 예약해야겠네요. 샌프란시스코행 비행편도 알아볼까요?'
        },
        {
          name:'실비:',
          speech:'음, 네, 괜찮으시다면요.'
        },
        {
          name:'마이클:',
          speech:'네, 문제없어요. 점심 식사 후에 인터넷으로 알아보고, 음… 다시 전화할게요. 호텔을 예약하는 것은 어떨까요?'
        },
        {
          name:'실비:',
          speech:'음, 그럼 샌프란시스코 지사에 연락해서 그들이 좋은 곳을 알고 있는지 알아볼까요? 리타와 연락할 수 있어요.'
        },
        {
          name:'마이클:',
          speech:'네, 좋은 생각이에요.'
        },
        {
          name:'실비:',
          speech:'오늘 오후에 사무실이 여는대로 전화할게요.'
        },
        {
          name:'마이클:',
          speech:'좋아요. 그러면 저는 비행기에 대해 알아보도록 하겠습니다. 그리고, 음… 다시 연락드리겠습니다.'
        },
        {
          name:'실비:',
          speech:'좋아요. 4시 30분쯤에 얘기할까요?'
        },
        {
          name:'마이클:',
          speech:'네, 좋아요. 그때 전화할게요.'
        },
        {
          name:'실비:',
          speech:'안녕히 계세요.'
        },
        {
          name:'마이클:',
          speech:'전화 주셔서 감사 해요 실비. 안녕히 계세요.'
        },
        ],

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
