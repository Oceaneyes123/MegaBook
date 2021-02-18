<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/hotel-registration_1098-14040.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Staying at a hotel

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
        Make sentences with the correct form of have got.
      </p>

      <ol style="margin: 12px;">
        <li>
           Do you have the bill?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          We have a reservation for two nights.<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          The receptionist has a message for you.<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
      </ol>
      <p>
        Free response:<br />
        alk about your best and worst experiences of staying in hotels. Why were they good or bad?
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
                    Fhave got
                  </p>
                  <p>
                    긍정문<br />
                    I'<b>ve got</b> a credit card.
                  </p>
                  <p>
                    부정문<br />
                    We <b>haven't got</b> a reservation.
                  </p>
                  <p>
                    의문형<br />
                    <b>Have</b> you <b>got</b> his number?
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
          name:'Kristi:',
          speech:' Hello. I’ve got a reservation. Kristi Cortland.'
        },
        {
          name:'Rec:',
          speech:'Ms Cortland... a single room, for three nights?'
        },
        {
          name:'Kristi:',
          speech:'That’s right.'
        },
        {
          name:'Rec:',
          speech:'OK. Could you fill in this form, please?'
        },
        {
          name:'Kristi:',
          speech:'Sure. Have you got a pen?'
        },
        {
          name:'Rec:',
          speech:'Yes. Here you are.'
        },
        {
          name:'Kristi:',
          speech:'Thanks. Um... It says ’company account number’. I haven’t got the number. My company made the reservation, but, um, I don’t...'
        },
        {
          name:'Rec:',
          speech:'It doesn’t matter. You don’t need to write that. Just put your name, address, passport number, and signature. That’s fine.'
        },
        {
          name:'Kristi:',
          speech:'OK.'
        },
        {
          name:'Rec:',
          speech:'This is the card for your room.'
        },
        {
          name:'Kristi:',
          speech:'To open the door?'
        },
        {
          name:'Rec:',
          speech:'Yes. You just insert the card, and the door opens automatically.'
        },
        {
          name:'Kristi:',
          speech:'Right. OK.'
        },
        {
          name:'Rec:',
          speech:'It’s room three one five, on the third floor.'
        },
        {
          name:'Kristi:',
          speech:'Right.'
        },
        {
          name:'Rec:',
          speech:'In the morning, breakfast is from six-thirty to ten.'
        },
        {
          name:'Kristi:',
          speech:'From six-thirty. Right.'
        },
        {
          name:'Rec:',
          speech:'The dining room’s just over there.'
        },
        {
          name:'Kristi:',
          speech:'OK.'
        },
        {
          name:'Rec:',
          speech:'We’ve got twenty-four-hour room service. Just dial nine from your room.'
        },
        {
          name:'Kristi:',
          speech:'Right.'
        },
        {
          name:'Rec:',
          speech:'Would you like a wake-up call?'
        },
        {
          name:'Kristi:',
          speech:'Um...no. No, thanks.'
        },
        {
          name:'Rec:',
          speech:'OK. And you’ve got a message from Mr Soga. He says he’s coming to the hotel at seven forty-five.'
        },
        {
          name:'Kristi:',
          speech:'Seven forty-five. Right. OK, thanks very much.'
        },
        {
          name:'Rec:',
          speech:'You’re welcome. Have a nice day.'
        },
        {
          name:'Kristi:',
          speech:'Thanks.'
        },
        ],

        translations:[
        {
          name:'크리스티:',
          speech:'안녕하세요. 저 예약을 했습니다. 크리스티 코트랜드로.'
        },
        {
          name:'레크:',
          speech:'코트랜드 양... 싱글 룸으로 3박맞으신가요?'
        },
        {
          name:'크리스티:',
          speech:'맞아요.'
        },
        {
          name:'레크:',
          speech:'알겠습니다. 이 양식을 작성해 주시겠습니까?'
        },
        {
          name:'크리스티:',
          speech:'물론이죠. 펜을 가지고 있으신가요?'
        },
        {
          name:'레크:',
          speech:'네. 여기 있습니다.'
        },
        {
          name:'크리스티:',
          speech:'고맙습니다. 음…’회사 계좌번호’라고 적혀있어요. 저는 그 번호를 모릅니다. 우리 회사가 예약했는데, 음, 난...'
        },
        {
          name:'레크:',
          speech:'그건 중요하지 않아요. 그거 쓸 필요 없어요. 이름, 주소, 여권 번호, 서명만 하면 돼요. 괜찮습니다.'
        },
        {
          name:'크리스티:',
          speech:'알았어요.'
        },
        {
          name:'레크:',
          speech:'이것은 당신의 방 카드 입니다.'
        },
        {
          name:'크리스티:',
          speech:'문을 열기위한?'
        },
        {
          name:'레크:',
          speech:'네. 카드를 넣으면 자동으로 문이 열립니다.'
        },
        {
          name:'크리스티:',
          speech:'그렇군요'
        },
        {
          name:'레크:',
          speech:'3층 315호실입니다.'
        },
        {
          name:'크리스티:',
          speech:'그렇군요.'
        },
        {
          name:'레크:',
          speech:'아침 식사는 6시 30분부터 10시까지입니다.'
        },
        {
          name:'크리스티:',
          speech:'6시 30분부터. 알겠습니다.'
        },
        {
          name:'레크:',
          speech:'식당은 바로 저쪽에 있어요.'
        },
        {
          name:'크리스티:',
          speech:'알겠어요.'
        },
        {
          name:'레크:',
          speech:' 24시간 룸서비스가 있습니다. 방에서 9번을 누르세요.'
        },
        {
          name:'크리스티:',
          speech:'알겠습니다.'
        },
        {
          name:'레크:',
          speech:'모닝콜 하시겠습니까?'
        },
        {
          name:'크리스티:',
          speech:'음...아니요. 사양하겠습니다.'
        },
        {
          name:'레크:',
          speech:'알겠습니다. 그리고 소가 씨한테서 전갈을 받았습니다. 그는 7시 45분에 호텔로 온다고 합니다.'
        },
        {
          name:'크리스티:',
          speech:'7시 45분. 그렇군요. 고마워요'
        },
        {
          name:'레크:',
          speech:'천만에요. 좋은 하루 보내세요.'
        },
        {
          name:'크리스티:',
          speech:'고마워요.'
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
