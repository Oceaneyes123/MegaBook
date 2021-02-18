<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/portrait-man-working-desk-with-laptop_1163-2105.jpg" class="cover-photo">

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
        padding-bottom: 10px;">What have you done?
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">What have you done?</li><br />

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
            Have you washed your hair today?
          </li>
          <li>
            Have you called a friend today?
          </li>
          <li>
            Have you been shopping this week?
          </li>
          <li>
            Have you watched TV this weekend?
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
                      완료를 나타내는 현재완료 : 과거에 시작된 행동이 지금 막 완료되었을 때 사용이 되며 이 때 just, yet, already와 같은 부사와 함께 자주 쓰입니다.<br />
                      already : 평서문 에서는 이미 ~했다, 의문문에서는 놀라거나 실망해서 벌써 ~했습니까?로 해석이 됩니다.<br />                  
                      yet : 부정문에는 아직 ~하지 않았다, 의문문에서는 어떤 일이 지금쯤은 끝났을 것으로 기대할 때 사용되며 해석은 따로 하지 않습니다.<br />
                    </li>
                    <li>
                      you've done a good job : 일을 잘했어. 일을 잘 처리했어.<br />
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
          speech:'Oh, no!'
        },
        {
          name:'B:',
          speech:'What’s wrong?'
        },
        {
          name:'A:',
          speech:'I can’t find my pen.'
        },
        {
          name:'B:',
          speech:'Really? Ha ha ha.'
        },
        {
          name:'A:',
          speech:'It isn’t funny.'
        },
        {
          name:'B:',
          speech:'Oh, yes it is.'
        },
        {
          name:'A:',
          speech:'It is? I don’t understand.'
        },
        {
          name:'B:',
          speech:'Well, you have to look carefully.'
        },
        {
          name:'A:',
          speech:'I’ve looked everywhere.'
        },
        {
          name:'B:',
          speech:'No, you haven’t. Look behind your ear.'
        },
        {
          name:'A:',
          speech:'Oh.'
        },
        {
          name:'  ',
          speech:'  '
        },
        {
          name:'C:',
          speech:'Watch out! I’ve just washed the floor.'
        },
        {
          name:'D:',
          speech:'No, you haven’t.'
        },
        {
          name:'C:',
          speech:'Yes, I have.'
        },
        {
          name:'D:',
          speech:'Well, you haven’t done a very good job. Look over there. You’ve missed a spot.'
        },
        {
          name:'C:',
          speech:'You’re right. Here’s the mop.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'I’m so bored.'
        },
        {
          name:'F:',
          speech:'Well, do something.'
        },
        {
          name:'E:',
          speech:'What, for example?'
        },
        {
          name:'F:',
          speech:'Wash your hair.'
        },
        {
          name:'E:',
          speech:'I’ve already washed it.'
        },
        {
          name:'F:',
          speech:'Call your friend Susan.'
        },
        {
          name:'E:',
          speech:'I’ve already talked to her today.'
        },
        {
          name:'F:',
          speech:'Clean your room.'
        },
        {
          name:'E:',
          speech:'I’ve already cleaned it.'
        },
        {
          name:'F:',
          speech:'Then do the dishes.'
        },
        {
          name:'E:',
          speech:'Haven’t you done them yet?'
        },
        {
          name:'F:',
          speech:'No, I haven’t.'
        },
        {
          name:'E:',
          speech:'Oh, all right.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'이런, 안 돼요!'
        },
        {
          name:'B:',
          speech:'왜 그래요?'
        },
        {
          name:'A:',
          speech:'제 펜을 찾을 수가 없어요.'
        },
        {
          name:'B:',
          speech:'정말? 하하하'
        },
        {
          name:'A:',
          speech:'재미없어요.'
        },
        {
          name:'B:',
          speech:'아, 그래요.'
        },
        {
          name:'A:',
          speech:'그래요? 이해가 안 돼요.'
        },
        {
          name:'B:',
          speech:'음, 잘 보세요.'
        },
        {
          name:'A:',
          speech:'사방을 다 찾아봤어요.'
        },
        {
          name:'B:',
          speech:'아뇨, 안 그랬어요. 귀 뒤를 보세요.'
        },
        {
          name:'A:',
          speech:'오.'
        },
        {
          name:'  ',
          speech:'  '
        },
        {
          name:'C:',
          speech:'조심해요! 방금 바닥을 씻었어요.'
        },
        {
          name:'D:',
          speech:'아뇨, 안 그랬어요.'
        },
        {
          name:'C:',
          speech:'네, 있습니다.'
        },
        {
          name:'D:',
          speech:'음, 당신은 일을 잘 못 해냈군요. 저기를 보세요. 자리를 놓쳤어요.'
        },
        {
          name:'C:',
          speech:'맞아요. 여기 대걸레가 있습니다.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'너무 지루해요.'
        },
        {
          name:'F:',
          speech:'뭐, 어떻게 좀 해보세요.'
        },
        {
          name:'E:',
          speech:'예를 들면요?'
        },
        {
          name:'F:',
          speech:'재미없어요.'
        },
        {
          name:'E:',
          speech:'벌써 씻었어요.'
        },
        {
          name:'F:',
          speech:'친구 Susan에게 전화하세요.'
        },
        {
          name:'E:',
          speech:'오늘 이미 그녀와 얘기했어요.'
        },
        {
          name:'F:',
          speech:'방을 청소하세요.'
        },
        {
          name:'E:',
          speech:'이미 청소했어요.'
        },
        {
          name:'F:',
          speech:'그럼 설거지를 하세요.'
        },
        {
          name:'E:',
          speech:'아직 안 했어요?'
        },
        {
          name:'F:',
          speech:'아니요, 못 봤어요.'
        },
        {
          name:'E:',
          speech:'아, 알았어요.'
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
