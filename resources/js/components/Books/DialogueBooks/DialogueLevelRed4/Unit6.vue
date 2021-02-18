<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/side-view-woman-singing-microphone-wearing-headphones_23-2148366443.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Superstar
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Superstar</li><br />

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
            What does Maria-Donna want Marvin to do?<br />
          </li>
          <li>
            What does she want Brandon to do?<br />
          </li>
          <li>
            What does she want Tania and Sophie to sing?<br />
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
                      to부정사 : 5형식 문장에서 동사의 목적격보어로 쓰이기도 합니다<br />
                            want + 목적어 + to부정사 : ~가 ~하는 것을 바라다<br />
                        <br />
                        Ex) I want you to ready a car for this afternoon : 나는 오늘 오후에 당신이 차를 준비시켜주기를 원해요<br />
                            I want you to play electric piano : 나는 당신이 전자 기타를 치기를 원해요<br />
                            I want Jared to play acoustic guitar : 나는 당신이 어쿠스틱 기타를 치기를 원해요<br />
                            I want him to play real loudly : 나는 그가 진짜 크게 치기를 원해요<br />
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
          name:'Maria-Donna:',
          speech:'Come in!'
        },
        {
          name:'Gary:',
          speech:'Yes, Ms. Baloney?'
        },
        {
          name:'Maria-Donna:',
          speech:'No, no, Gary! I don’t want you.'
        },
        {
          name:'Gary:',
          speech:'Who do you want, Ms. Baloney?'
        },
        {
          name:'Maria-Donna:',
          speech:'I want Marvin, and I want him right away.'
        },
        {
          name:'Gary:',
          speech:'OK. I’ll go and find him.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Maria-Donna:',
          speech:'Ah, Marvin!'
        },
        {
          name:'Marvin:',
          speech:'Did you want to see me, ma’am?'
        },
        {
          name:'Maria-Donna:',
          speech:'Yes. I wanted to see you twenty minutes ago.'
        },
        {
          name:'Marvin:',
          speech:'I’m sorry. I was in the garage.'
        },
        {
          name:'Maria-Donna:',
          speech:'I want you to ready a car for this afternoon.'
        },
        {
          name:'Marvin:',
          speech:'Which car do you want to take? The stretch limo, the Rolls-Royce, or the Ferrari?'
        },
        {
          name:'Maria-Donna:',
          speech:'The stretch limo.'
        },
        {
          name:'Marvin:',
          speech:'Where do you want to go, ma’am?'
        },
        {
          name:'Maria-Donna:',
          speech:'The recording studio.'
        },
        {
          name:'Marvin:',
          speech:'What time?'
        },
        {
          name:'Maria-Donna:',
          speech:'The recording session begins at two. We’ll leave here at one-thirty.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Maria-Donna:',
          speech:'OK, Brandon. Can you hear me?'
        },
        {
          name:'Brandon:',
          speech:'Sure.'
        },
        {
          name:'Maria-Donna:',
          speech:'I want you to play electric piano.'
        },
        {
          name:'Brandon:',
          speech:'No problem.'
        },
        {
          name:'Maria-Donna:',
          speech:'And I want Jared to play acoustic guitar. I want him to play real loudly, OK?'
        },
        {
          name:'Brandon:',
          speech:'You got it.'
        },
        {
          name:'Maria-Donna:',
          speech:'And find Tania and Sophie. I want them to sing doo-wops.'
        },
        {
          name:'Brandon:',
          speech:'Excuse me?'
        },
        {
          name:'Maria-Donna:',
          speech:'You know, the chorus. Doo-wop-di-diddy-diddy-dum-di-do.'
        },
        ],

        translations:[
        {
          name:'Maria-Donna:',
          speech:'들어오세요!'
        },
        {
          name:'Gary:',
          speech:'네, Baloney씨? 네, Baloney씨요?'
        },
        {
          name:'Maria-Donna:',
          speech:'안 돼요, Gary! 난 당신을 원하지 않아요.'
        },
        {
          name:'Gary:',
          speech:'Baloney씨, 누구를 원하세요?'
        },
        {
          name:'Maria-Donna:',
          speech:'입니다. 난 Marvin을 원해요 그리고 난 당장 그를 원해요'
        },
        {
          name:'Gary:',
          speech:'알았어요. 제가 가서 그를 찾을게요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Maria-Donna:',
          speech:'입니다. 아, Marvin이에요!'
        },
        {
          name:'Marvin:',
          speech:'부인, 저를 보자고 하셨나요?'
        },
        {
          name:'Maria-Donna:',
          speech:'네. 20분 전에 뵙고 싶었어요.'
        },
        {
          name:'Marvin:',
          speech:'죄송합니다. 차고에 있었어요'
        },
        {
          name:'Maria-Donna:',
          speech:'입니다. 오늘 오후에 쓸 차를 준비해 주세요.'
        },
        {
          name:'Marvin:',
          speech:'어떤 차를 타시겠어요? 스트레치 리무진, 롤스로이스, 아니면 페라리요?'
        },
        {
          name:'Maria-Donna:',
          speech:'입니다. 스트레치 리무진입니다.'
        },
        {
          name:'Marvin:',
          speech:'부인, 어디로 가고 싶습니까?'
        },
        {
          name:'Maria-Donna:',
          speech:'녹음실입니다.'
        },
        {
          name:'Marvin:',
          speech:'몇 시에요?'
        },
        {
          name:'Maria-Donna:',
          speech:'녹음 세션은 2시에 시작됩니다. 우리는 1시 30분에 여기를 떠날 거예요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Maria-Donna:',
          speech:'알겠어요, Brandon. 내 말 들려요?'
        },
        {
          name:'Brandon:',
          speech:'은 다음과 같이 말합니다. 물론이죠'
        },
        {
          name:'Maria-Donna:',
          speech:'입니다. 나는 당신이 전자 피아노를 연주했으면 좋겠어요.'
        },
        {
          name:'Brandon:',
          speech:'은 다음과 같이 말합니다. 문제없습니다'
        },
        {
          name:'Maria-Donna:',
          speech:'입니다. 그리고 저는 제러드가 통기타를 연주했으면 좋겠어요. 그가 정말 크게 연주했으면 좋겠어요, 알았죠?'
        },
        {
          name:'Brandon:',
          speech:'알겠습니다.'
        },
        {
          name:'Maria-Donna:',
          speech:'입니다. 그리고 Tania와 Sophie를 찾으세요. 나는 그들이 doo-wops을 부르길 원해요.'
        },
        {
          name:'Brandon:',
          speech:'뭐라고요?'
        },
        {
          name:'Maria-Donna:',
          speech:'입니다. 후렴구 있잖아요. Doo-wop-di-diddy-diddy-dum-dum-di-do.'
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
