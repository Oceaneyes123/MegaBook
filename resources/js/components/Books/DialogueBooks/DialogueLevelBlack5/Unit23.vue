<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/football-fans-stadium-from_23-2147844564.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Football Game
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Football Game</li><br />

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
          <u>Complete the sentences using may or might + an appropriate verb in the box. Use each verb only once</u><br />
        </p>
        <br />
        <p>
          Ex) Carla is very busy. She may miss the football game tomorrow.
        </p>
        <v-container grid-list-md text-xs-center>
          <v-layout wrap align-content-center>

            <v-flex xs12 md4 >
              <v-card hover>

                <v-img src="images/dialogue-books-anne.png" />

              </v-card>
            </v-flex>

          </v-layout>
        </v-container>
        <ol style="margin: 12px;">
          <li>
            My sister loves to cook. She <u> &emsp; &emsp; &emsp; </u><u> &emsp; &emsp; &emsp; </u> a restaurant someday. <br />
          </li>
          <li>
            Stanley is worried. He <u> &emsp; &emsp; &emsp; </u><u> &emsp; &emsp; &emsp; </u> his job at the post office. <br />
          </li>
          <li>
            It’s getting cloudy. It <u> &emsp; &emsp; &emsp; </u><u> &emsp; &emsp; &emsp; </u> today. <br />
          </li>
          <li>
            We’re having problems with our car. We <u> &emsp; &emsp; &emsp; </u><u> &emsp; &emsp; &emsp; </u> it and get a new one. <br />
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
                      조동사 may : 상대방에서 허가를 구하거나 허가를 할 때<br />
                                    현재나 미래의 일에 대한 불확실한 추측이나 가능성을 나타낼 때<br />
                    </li>
                    <li>
                      조동사 might : may와 마찬가지로 현재나 미래의 일에 대한 불확실한 추측이나 가능성을 나타낼 때<br />
                                     may에 비해 더욱 불확실한 상황에 쓰이는 경우가 있지만, 보통 둘은 큰 의미 차이가 없이 쓰입니다.<br />
                                     Example:<br />
                                        I may go, or I may not : 나는 아마 갈 수 있을 지도 갈 수 없을지도 모릅니다<br />
                                        It may rain tomorrow : 내일 비가 올지도 모릅니다<br />
                                        They might win : 그들은 이길런지도 모릅니다<br />
                                        You may be right : 너가 옳을지도 몰라<br />
                                        She might go : 그녀는 갈런지도 몰라<br />
                                        This may come as a surprise to you : 이것은 너에게 놀라운 일처럼 다가올런지 모른다 <br />
                    </li>
                    <li>
                      make up one's mind : ~을 결심하다, 체념하다
                    </li>
                    <li>
                      "it depends on the weather" : 그것은 날씨에 달려 있습니다
                    </li>
                    <li>
                      make a suggestion : 제안을 하다
                    </li>
                    <li>
                      "anything is possible" : 무엇이든 가능하다
                    </li>
                    <li>
                      as if : 마치 ~처럼
                    </li>
                    <li>
                      for anything : 결코, 절대로, 무슨 일이 있어도 (I wouldn’t miss tomorrow’s game for anything : 나는 무슨 일이 있어도 내일 게임은 놓치지 않을거야)
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
          speech:'Are you going to see the big football game tomorrow?'
        },
        {
          name:'B:',
          speech:'I may go, or I may not.'
        },
        {
          name:'A:',
          speech:'Why can’t you make up your mind?'
        },
        {
          name:'B:',
          speech:'Well, it depends on the weather. It may rain tomorrow, and I don’t like to sit in the rain'
        },
        {
          name:'A:',
          speech:'Can I make a suggestion? Take an umbrella.'
        },
        {
          name:'B:',
          speech:'That’s an idea!'
        },
        {
          name:'A:',
          speech:'Say, do you think our team will win the game tomorrow?'
        },
        {
          name:'B:',
          speech:'I don’t know. They might win. Anything is possible.'
        },
        {
          name:'A:',
          speech:'I don’t see how we can lose. We have the best players.'
        },
        {
          name:'B:',
          speech:'You may be right. You certainly have a right to your opinion.'
        },
        {
          name:'A:',
          speech:'Hey, you sound as if you don’t care who wins the game.'
        },
        {
          name:'B:',
          speech:'This may come as a surprise to you, Joe, but I’m not very interested in football.'
        },
        {
          name:'A:',
          speech:'Well, I wouldn’t miss tomorrow’s game for anything.'
        },
        {
          name:'B:',
          speech:'Is your girlfriend going with you?'
        },
        {
          name:'A:',
          speech:'I don’t know. She might go. Her interest in football is about the same as yours'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'내일 큰 축구 경기 보러 갈 거예요?'
        },
        {
          name:'B:',
          speech:'갈 수도 있고 안 갈 수도 있어요.'
        },
        {
          name:'A:',
          speech:'왜 결정을 못 내려요?'
        },
        {
          name:'B:',
          speech:'글쎄요, 날씨에 따라 다르죠. 내일 비가 올지도 모르고, 저는 비를 맞으며 앉아 있는 것을 좋아하지 않아요'
        },
        {
          name:'A:',
          speech:'제가 제안 하나 해도 될까요? 우산을 가지고 가세요.'
        },
        {
          name:'B:',
          speech:'좋은 생각이에요!'
        },
        {
          name:'A:',
          speech:'저기, 우리 팀이 내일 경기에서 이길 것 같아요?'
        },
        {
          name:'B:',
          speech:'모르겠어요. 그들이 이길지도 몰라요. 무엇이든 가능합니다.'
        },
        {
          name:'A:',
          speech:'우리가 어떻게 질 수 있는지 모르겠어요. 우리에겐 최고의 선수들이 있습니다.'
        },
        {
          name:'B:',
          speech:'당신 말이 맞을지도 몰라요. 당신은 확실히 당신의 의견에 대한 권리가 있습니다.'
        },
        {
          name:'A:',
          speech:'이봐요, 누가 경기에서 이기든 상관없는 것처럼 말하네요.'
        },
        {
          name:'B:',
          speech:'조, 이것은 여러분에게 놀라운 일이 될 수도 있지만, 저는 축구에는 별로 관심이 없어요.'
        },
        {
          name:'A:',
          speech:'뭐, 내일 경기는 어떤 일이 있어도 놓치지 않을 거예요.'
        },
        {
          name:'B:',
          speech:'여자친구도 같이 가나요?'
        },
        {
          name:'A:',
          speech:'모르겠어요. 그녀가 갈지도 몰라요. 그녀의 축구에 대한 관심은 당신과 거의 같습니다.'
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
