<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/boy-is-confused-knowing-where-go_1150-19707.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Nobody knows everything
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br />( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Nobody knows everything</li><br />
     
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
          <u>Fill the blanks.</u><br />
          Ex) There’s something in my soup.<br />
        </p>
        <br />
        <p>
          something / someone / anything / anyone<br />
        </p>
        <br />
        <ol style="margin: 12px;">
          <li>
            There's <u> &emsp; &emsp; &emsp; </u> in the room. <br />
          </li>
          <li>
            Is there <u> &emsp; &emsp; &emsp; </u> in the refrigerator? <br />
          </li>
          <li>
            Is there <u> &emsp; &emsp; &emsp; </u> in the bathroom? <br />
          </li>
          <li>
            There isn't <u> &emsp; &emsp; &emsp; </u> in the cabinet. <br />
          </li>
        </ol>
        <br />
        <p>
          anywhere / everywhere / nothing / something<br />
        </p>
        <br />
        <ol style="margin: 12px;">
          <li>
            I looked <u> &emsp; &emsp; &emsp; </u>, but I can’t find it. <br />
          </li>
          <li>
            There’s <u> &emsp; &emsp; &emsp; </u> to eat for dinner. <br />
          </li>
          <li>
            Would you like <u> &emsp; &emsp; &emsp; </u> to drink? <br />
          </li>
          <li>
            I want to stay home. I don’t want to go <u> &emsp; &emsp; &emsp; </u>. <br />
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
                      사역동사 Let : let이 사역동사로 쓰여 ~시키다로 해석이 될 때에는 목적격보어로 동사의 원형이 옵니다. <br />
                    </li>
                    <li>
                      some, any : 몇몇, 약간의 뜻인데 some은 긍정문,평서문,권유문에 사용되고 any는 부정문에 사용됩니다.<br />
                    </li>
                    <li>
                      Are there any left? : 남은 것이 있나요?<br />
                    </li>
                    <li>
                      Every seat is reserved : 모든 좌석이 예약되다<br />
                    </li>
                    <li>
                      have a look : 한 번 보다<br />
                    </li>
                    <li>
                      look for : ~을 찾다<br />
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
          speech:'Good morning.'
        },
        {
          name:'B:',
          speech:'Good morning. How can I help you?'
        },
        {
          name:'A:',
          speech:'I want some seats for Tuesday night. Are there any left?'
        },
        {
          name:'B:',
          speech:'No, I’m very sorry. There are no seats left. Every seat is reserved.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'Doctor, I think there’s something in my eye.'
        },
        {
          name:'D:',
          speech:'Let me have a look.'
        },
        {
          name:'C:',
          speech:'Everything looks funny and it hurts.'
        },
        {
          name:'D:',
          speech:'I can’t see anything. No, I’m sure there’s nothing there.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'There’s somebody in the other office!'
        },
        {
          name:'F:',
          speech:'I didn’t hear anybody.'
        },
        {
          name:'E:',
          speech:'Take a look, please.'
        },
        {
          name:'F:',
          speech:'OK. No, there’s nobody there. Everybody went home.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'G:',
          speech:'What are you looking for?'
        },
        {
          name:'H:',
          speech:'My pen. It’s somewhere in this room.'
        },
        {
          name:'G:',
          speech:'Have you looked everywhere?'
        },
        {
          name:'H:',
          speech:'Yes, but I can’t find it anywhere.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'좋은 아침이에요.'
        },
        {
          name:'B:',
          speech:'좋은 아침이에요. 무엇을 도와드릴까요?'
        },
        {
          name:'A:',
          speech:'화요일 밤에 앉을 자리 좀 주세요. 남은 거 있어요?'
        },
        {
          name:'B:',
          speech:'아니요, 정말 죄송합니다. 좌석이 남아있지 않습니다. 모든 좌석은 예약되어 있습니다.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'의사선생님, 눈에 뭐가 들어간 것 같아요.'
        },
        {
          name:'D:',
          speech:'제가 한번 볼게요.'
        },
        {
          name:'C:',
          speech:'모든 게 재미있어 보이고 아파요.'
        },
        {
          name:'D:',
          speech:'아무것도 안 보여요. 아뇨, 거기엔 아무것도 없을 거예요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'다른 사무실에 누가 있어요!'
        },
        {
          name:'F:',
          speech:'아무도 못 들었어요.'
        },
        {
          name:'E:',
          speech:'한 번 봐주세요.'
        },
        {
          name:'F:',
          speech:'좋아요. 거기엔 아무도 없어요. 모두 집으로 돌아갔습니다.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'G:',
          speech:'뭘 찾으세요?'
        },
        {
          name:'H:',
          speech:'제 펜입니다. 이 방 어딘가에 있어요.'
        },
        {
          name:'G:',
          speech:'구석구석 찾아봤어요?'
        },
        {
          name:'H:',
          speech:'네, 하지만 어디에서도 찾을 수가 없어요.'
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
