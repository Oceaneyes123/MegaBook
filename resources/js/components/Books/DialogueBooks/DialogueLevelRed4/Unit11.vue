<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/sick-man-sweater-scarf-holding-cup-tea-while-having-cough_171337-4445.jpg" class="cover-photo">

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
        padding-bottom: 10px;">You should take some medicine
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">You should take some medicine</li><br />

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

        <ol style="margin: 12px;">
          <li>
            What do you do when you have a cold?<br />
          </li>
          <li>
            Imagine your teacher has a bad cold. Offer some recommendations.<br />
            <br />
            Example:<br />
              You should <u> &emsp; &emsp; &emsp; </u>.<br />
              It’s important to <u> &emsp; &emsp; &emsp; </u>.<br />
              It’s helpful to <u> &emsp; &emsp; &emsp; </u>.<br />
              It’s a good idea to <u> &emsp; &emsp; &emsp; </u>.<br />
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
                      to부정사의 명사적 용법 : to부정사가 문장에서 명사처럼 주어,목적어,보어의 역할을 합니다.<br />
                        Ex) To get a lot of rest is really important : 많이 쉬는 것이 정말 중요합니다.<br />
                        하지만 영어는 예문처럼 주어 부분이 길어지는 것을 좋아하지 않기 때문에 to부정사를 뒤로 보내고 가짜 주어인 it을 주어로 씁니다.<br />
                        가짜 주어인 it을 가주어, 진짜 주어인 to부정사를 진주어라고 하며, it은 해석하지 않습니다.<br />
                        <br />
                        It is really important to get a lot of rest (it - 가주어, to get 이하 -진주어) - To get a lot of rest is really important.<br />
                        It's sometimes helpful to eat garlic - To eat garlic is sometimes helpful.<br />
                        It's important to drink a lot of liquids - To drind a lot of liquids is important. <br />
                        It's a good idea to take some cold medicine - To take some cold medicine is a good idea. <br />
                    </li>
                    <li>
                      사역동사 : ~하도록 하다, 시키다는 의미의 동사이고 사역동사 다음에는 목적어와 목적격 보어가 뒤 따릅니다. 목적격 보어로는 동사원형을 사용합니다.<br />
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
          name:'A:',
          speech:'Hi Craig! How are you?'
        },
        {
          name:'B:',
          speech:'Not so good. I have a terrible cold.'
        },
        {
          name:'A:',
          speech:'Really? That’s too bad! You should be at home in bed. It’s really important to get a lot of rest.'
        },
        {
          name:'B:',
          speech:'Yeah, you’re right.'
        },
        {
          name:'A:',
          speech:'And you didn’t take anything for it, did you?'
        },
        {
          name:'B:',
          speech:'No, I didn’t.'
        },
        {
          name:'A:',
          speech:'I thought so. Well, it’s sometimes helpful to eat garlic and cook it in chicken stock. Try it! It really works!'
        },
        {
          name:'B:',
          speech:'Yuck! That sounds awful!'
        },
        {
          name:'',
          speech:''
        },
        {
          name:'C:',
          speech:'That cold sounds pretty bad, Craig!'
        },
        {
          name:'B:',
          speech:'Yeah, it is. Don’t get too close.'
        },
        {
          name:'C:',
          speech:'Well, you know, it’s important to drink a lot of liquids. I have some herbal tea. Let me make you a cup.'
        },
        {
          name:'B:',
          speech:'Oh, OK. That sounds good.'
        },
        {
          name:'',
          speech:''
        },
        {
          name:'D:',
          speech:'How’s that cold, Craig?'
        },
        {
          name:'B:',
          speech:'Not so good. I still have it.'
        },
        {
          name:'D:',
          speech:'Oh, too bad. Well, listen, it’s a good idea to take some cold medicine. And you should go home and take a long, hot bath.'
        },
        {
          name:'B:',
          speech:'You’re right. Maybe I should. Thanks for the advice.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'Craig 안녕하세요! 잘 지내시나요?'
        },
        {
          name:'B:',
          speech:'별로 안 좋아요. 나는 지독한 감기에 걸렸어요'
        },
        {
          name:'A:',
          speech:'그래요? 안됐군요! 당신은 집에서 침대에 누워 있어야 합니다. 휴식을 많이 취하는 것이 정말 중요해요.'
        },
        {
          name:'B:',
          speech:'네, 맞아요.'
        },
        {
          name:'A:',
          speech:'그리고 당신은 그것에 대해 아무것도 받아들이지 않았죠, 그렇죠'
        },
        {
          name:'B:',
          speech:'아뇨, 안 그랬어요.'
        },
        {
          name:'A:',
          speech:'그럴 줄 알았어요. 음, 마늘을 먹고 닭육수에 넣어 조리하면 도움이 될 때가 있어요. 한 번 해 보세요! 정말 효과가 있어요!'
        },
        {
          name:'B:',
          speech:'아이고, 아이고, 아이고! 그거 끔찍하게 들리네요!'
        },
        {
          name:'',
          speech:''
        },
        {
          name:'C:',
          speech:'그 추위는 꽤 안 좋은 것 같아요, Craig !'
        },
        {
          name:'B:',
          speech:'네, 그렇습니다. 너무 가까이 가지 마세요.'
        },
        {
          name:'C:',
          speech:'음, 아시다시피, 액체를 많이 마시는 것이 중요해요. 허브차가 좀 있어요. 내가 당신에게 한 잔 만들어 줄게요.'
        },
        {
          name:'B:',
          speech:'아, 알았어요. 그거 좋겠네요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'D:',
          speech:'Craig , 그렇게 추워요?'
        },
        {
          name:'B:',
          speech:'별로 안 좋아요. 아직 가지고 있어요.'
        },
        {
          name:'D:',
          speech:'아, 안됐군요. 음, 들어봐요, 감기약을 먹는 게 좋은 생각이에요. 그리고 당신은 집에 가서 길고 뜨거운 목욕을 해야 합니다.'
        },
        {
          name:'B:',
          speech:'맞아요. 그래야 할 것 같아요. 조언해 주셔서 감사합니다.'
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
