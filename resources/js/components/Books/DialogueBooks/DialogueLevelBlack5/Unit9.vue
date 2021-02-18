<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/man-woman-having-fun-standing_23-2147657117.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Opinions
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Opinions</li><br />

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
            What TV shows are you interested in? <br />
          </li>
          <li>
            What TV shows are you interested in? <br />
          </li>
          <li>
            Have you seen anything on TV that shocked you recently? <br />
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
                      형용사로 쓰이는 분사 : <br />
                      형용사처럼 쓰이는 현재분사(-ing) - 능동(~하는)이나 진행(~하고 있는)의 의미를 나타냅니다<br />
                      형용사처럼 쓰이는 과거분사(-ed) - 수동(~된)의 의미를 나타냅니다.<br />
                      주로 현재분사는 사물이 주어이거나 사물을 수식할 때, 과거분사는 사람이 주어이거나 사람을 수식할 때 쓰이지만, 항상 그런 것은 아닙니다.<br />
                      주어가 어떤 감정을 유발할 때는 현재분사를 쓰고, 어떤 감정을 느낄 때는 과거분사를 씁니다.<br />
                      =>  interesting (재미있는) / interested (재미를 느끼는)<br />
                          boring (지루한) / bored (지루해진)<br />
                          exciting (흥분시키는) / excited (흥분한)<br />
                          tiring (피곤하게 하는) / tired (피곤한)<br />
                          surprising (놀라운) / surprised (놀란)<br />
                          worrying (걱정스러운) / worried (걱정되는)<br />
                          shocking (충격적인) / shocked (충격받은)<br />
                    </li>
                    <li>
                      do a survey : 설문조사를 하다
                    </li>
                    <li>
                      most of : ~의 대부분
                    </li>
                    <li>
                      think of : ~에 관심을 보이다, ~에 마음을 쓰다, ~을 상상하다, ~을 ~라고 생각하다
                    </li>
                    <li>
                      "it's very difficult to film animals" (= filming animals is very difficult) : 동물을 촬영하는 것은 매우 어렵다
                    </li>
                    <li>
                      pick up : 마중나가다
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
          name:'Interviewer:',
          speech:'Good afternoon. Mrs. Archer?'
        },
        {
          name:'Rita:',
          speech:'Yes?'
        },
        {
          name:'Int:',
          speech:'I’m from Channel Five TV. We’re doing a survey.'
        },
        {
          name:'Rita:',
          speech:'Oh, really?'
        },
        {
          name:'Int:',
          speech:'Could I ask you a few questions?'
        },
        {
          name:'Rita:',
          speech:'Well, uh...'
        },
        {
          name:'Int:',
          speech:'First, did you watch TV last night?'
        },
        {
          name:'Rita:',
          speech:'Yes, after dinner. From about seven o’clock.'
        },
        {
          name:'Int:',
          speech:'And did you watch any of our programs?'
        },
        {
          name:'Rita:',
          speech:'Yes, most of the evening. Till eleven.'
        },
        {
          name:'Int:',
          speech:'So you saw Animals in Focus. What did you think of it?'
        },
        {
          name:'Rita:',
          speech:'It was very interesting. I like wildlife programs.'
        },
        {
          name:'Int:',
          speech:'So you’re interested in wildlife?'
        },
        {
          name:'Rita:',
          speech:'Uh-huh. That kind of program always interests me. It’s very difficult to film animals, you know.'
        },
        {
          name:'Int:',
          speech:'What about your husband? Did he watch it?'
        },
        {
          name:'Rita:',
          speech:'Only for about five minutes. He’s not interested in animals. He says it’s boring.... Look, I’m very sorry, but I have to pick up the kids from school. Are there many more questions?'
        },
        ],

        translations:[
        {
          name:'진행자:',
          speech:'안녕하세요. Archer부인?'
        },
        {
          name:'Rita:',
          speech:'네?'
        },
        {
          name:'진행자:',
          speech:'저는 채널 5 TV에서 왔습니다. 설문조사를 하고 있습니다.'
        },
        {
          name:'Rita:',
          speech:'아, 그래요?'
        },
        {
          name:'진행자:',
          speech:'몇 가지 질문을 해도 될까요?'
        },
        {
          name:'Rita:',
          speech:'음, 음, 어...요.'
        },
        {
          name:'진행자:',
          speech:'우선, 어젯밤에 TV 봤어요?'
        },
        {
          name:'Rita:',
          speech:'네, 저녁 식사 후에요. 7시쯤부터요..'
        },
        {
          name:'진행자:',
          speech:'그리고 저희 프로그램을 보신 적이 있나요?'
        },
        {
          name:'Rita:',
          speech:'네, 대부분의 저녁 시간입니다. 11시까지요.'
        },
        {
          name:'진행자:',
          speech:'포커스의 동물을 보셨군요. 당신은 그것에 대해 어떻게 생각했나요?'
        },
        {
          name:'Rita:',
          speech:'매우 흥미로웠어요. 저는 야생동물 프로그램을 좋아합니다.'
        },
        {
          name:'진행자:',
          speech:'그럼 야생 동물에 관심이 있으신가요?'
        },
        {
          name:'Rita:',
          speech:'네, 그래요. 그런 프로그램은 언제나 흥미로워요. 아시다시피 동물을 촬영하는 것은 매우 어렵습니다.'
        },
        {
          name:'진행자:',
          speech:'당신 남편은요? 그가 그것을 봤나요?'
        },
        {
          name:'Rita:',
          speech:'5분 정도밖에 안 돼요. 그는 동물에 관심이 없어요. 지루하대요.... 이봐요, 정말 미안하지만, 학교에서 아이들을 데려와야 해요. 질문이 더 있습니까?'
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
