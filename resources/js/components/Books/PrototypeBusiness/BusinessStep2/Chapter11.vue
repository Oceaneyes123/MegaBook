<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/beautiful-girl-standing-airport_1157-22071.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Checking in for a flight
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border" >Today's topic</h3>
  <div style = "padding : 16px;">

  <table style = "border-collapse: collapse;">

    <tr v-for="dialog in dialogs" :key="dialog">
      <td class = "uppertable" >{{dialog.name}}</td>
      <td class = "lowertable" >{{dialog.speech}}</td>
    </tr>

  </table>

  
<div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Translation</h3>
  <div style="padding : 16px;">

    <table style = "border-collapse: collapse;">

      <tr v-for="translation in translations" :key="translation">
        <td class = "uppertable" >{{translation.name}}</td>
        <td class = "lowertable" >{{translation.speech}}</td>
      </tr>

    </table>
 </div>


<div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
</div>
<h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Exercise</h3>
<div style="padding : 16px;">

      <p>
        Answer the questions.
      </p>

      <ol style="margin: 12px;">
        <li>
          What identification does the man have?
        </li>
        <li>
          Does he get a window seat?
        </li>
        <li>
          Why is the plane full?
        </li>
        <li>
          Is the flight on time?
        </li>
        <li>
          Does the man have any luggage to check in?
        </li>
        <li>
          Which gate does he need to go to?
        </li>
        <li>
          Where are the shops?
        </li>
      </ol>
      <p>
        Free response:<br />
        Talk about your bad or funny experiences of travelling by plane.
      </p>
      <p>
        - delays<br />
        - cancellations<br />
        - lost luggage<br />
        - missing a flight><br />
        - forgetting your ticket or passport
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
                    some/any/no
                  </p>
                  <p>
                    의문형: any<br />
                    Do you have <b>any</b> information about the flight?
                  </p>
                  <p>
                    긍정문: some<br />
                    There are <b>some</b> passengers at the check-in.
                  </p>
                  <p>
                    부정문: no 또는 any<br />
                    I have <b>no</b> hand luggage.<br />
                    I don't have <b>any</b> hand luggage.
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
          name:'Stewardess:',
          speech:'Hello.'
        },
        {
          name:'Passenger:',
          speech:'Hello. Where did I put my ticket? Ah. There it is. Here you are.'
        },
        {
          name:'Stewardess:',
          speech:'Thank you. Do you have any ID?'
        },
        {
          name:'Passenger:',
          speech:'Sorry?'
        },
        {
          name:'Stewardess:',
          speech:'Do you have any identification? Your passport or an identity card...'
        },
        {
          name:'Passenger:',
          speech:'Oh yes. My passport. There you are. '
        },
        {
          name:'Stewardess:',
          speech:'Yes, this is fine. The plane’s quite full. The last flight was cancelled.'
        },
        {
          name:'Passenger:',
          speech:'Right. So is this flight on time?'
        },
        {
          name:'Stewardess:',
          speech:'Um... it’s delayed about ten minutes. Do you have any luggage?'
        },
        {
          name:'Passenger:',
          speech:'Just one case.'
        },
        {
          name:'Stewardess:',
          speech:'A suitcase?'
        },
        {
          name:'Passenger:',
          speech:'No, it’s just a briefcase. I’ll take it as hand luggage.'
        },
        {
          name:'Stewardess:',
          speech:'OK. So you have no luggage to check in.'
        },
        {
          name:'Passenger:',
          speech:'No. I don’t have any other bags.'
        },
        {
          name:'Stewardess:',
          speech:'OK, fine. Here’s your boarding pass.'
        },
        {
          name:'Passenger:',
          speech:'Thank you.'
        },
        {
          name:'Stewardess:',
          speech:'We’re boarding in... thirty-five minutes. Gate twelve B.'
        },
        {
          name:'Passenger:',
          speech:'Right. Um... are there any shops, after the security check?'
        },
        {
          name:'Stewardess:',
          speech:'No. There are some shops over there. Before you go through security.'
        },
        {
          name:'Passenger:',
          speech:'Oh, I see. OK, thank you.'
        },
        {
          name:'Stewardess:',
          speech:'You’re welcome.'
        },
        ],

        translations:[
        {
          name:'스튜어디스:',
          speech:'안녕하세요.'
        },
        {
          name:'승객:',
          speech:'안녕하세요. 내가 표를 어디에 뒀지? 아. 여기 있네. 여기요.'
        },
        {
          name:'스튜어디스:',
          speech:'고맙습니다. 신분증 있으십니까?'
        },
        {
          name:'승객:',
          speech:'네?'
        },
        {
          name:'스튜어디스:',
          speech:'신분을 증명할 만한 것을 가지고 계십니까? 여권이나 신분증...'
        },
        {
          name:'승객:',
          speech:'아 네 제 여권. 여기 있습니다.'
        },
        {
          name:'스튜어디스s:',
          speech:'그래, 이건 괜찮아. 비행기가 꽤 만원이다. 마지막 비행기가 취소되었다.'
        },
        {
          name:'승객:',
          speech:'네. 그럼 이 비행기는 정시에 도착하는 겁니까?'
        },
        {
          name:'스튜어디스:',
          speech:'음... 10분 정도 지연됐어요. 짐이 있으십니까?'
        },
        {
          name:'승객:',
          speech:'딱 하나요.'
        },
        {
          name:'스튜어디스:',
          speech:'여행가방이요?'
        },
        {
          name:'승객:',
          speech:'아니, 그냥 서류 가방입니다. 들고 탈 거예요.'
        },
        {
          name:'스튜어디스:',
          speech:'알겠습니다. 그러면 당신은 체크인할 짐이 없습니다.'
        },
        {
          name:'승객:',
          speech:'나는 다른 가방이 없습니다.'
        },
        {
          name:'스튜어디스:',
          speech:'네 알겠습니다. 여기 탑승권 입니다.'
        },
        {
          name:'승객:',
          speech:'고맙습니다.'
        },
        {
          name:'스튜어디스:',
          speech:'탑승하겠습니다... 35분 B 관문 12번.'
        },
        {
          name:'승객:',
          speech:'네. 보안 검사 후에 가게가 있나요?'
        },
        {
          name:'스튜어디스:',
          speech:'아니요. 저쪽에 가게가 몇 개 있습니다. 보안 검색을 하기 전에요.'
        },
        {
          name:'승객:',
          speech:'아, 그렇군요. 고마워요.'
        },
        {
          name:'스튜어디스:',
          speech:'천만에요.'
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
