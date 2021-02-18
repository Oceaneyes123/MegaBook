 <template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/young-funny-loving-couple-have-fun-sunny-day_146671-15055.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Date
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Date</li><br />

      <table style = "border-collapse: collapse;">
    
        <tr v-for="dialog in dialogs" :key="dialog">
          <td class = "uppertable" >{{dialog.name}}</td>
          <td class = "lowertable" >{{dialog.speech}}</td>
        </tr>
  
      </table>

      <br />
      <p>
        After the movie  
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="moviedialog in moviedialogs" :key="moviedialog">
          <td class = "uppertable" >{{moviedialog.name}}</td>
          <td class = "lowertable" >{{moviedialog.speech}}</td>
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
          <u>Talk about dating</u><br />
        </p>
        <br />
        <p>
          - Are young Koreans dating a lot?<br />
          - Where do they usually go? <br />
          - What was your best date? <br />
          - What was your worst date? <br />
        </p>


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

        <br />
        <p>
          영화가 끝난 후
        </p>
        <table style = "border-collapse: collapse;">
    
          <tr v-for="movietranslation in movietranslations" :key="movietranslation">
            <td class = "uppertable" >{{movietranslation.name}}</td>
            <td class = "lowertable" >{{movietranslation.speech}}</td>
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
                      "I was wondering if ..." : ~인지 생각하고 있었다<br />
                    </li>
                    <li>
                      pick up : 마중나가다
                    </li>
                    <li>
                      the best part : 가장 좋은 부분
                    </li>
                    <li>
                      "the only thing I didn't like" : 내가 싫었던 유일한 것
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
          speech:'Hello.'
        },
        {
          name:'B:',
          speech:'Hi, Linda. It’s Joe.'
        },
        {
          name:'A:',
          speech:'Joe! How are you?'
        },
        {
          name:'B:',
          speech:'Fine. Are you doing anything Friday night?'
        },
        {
          name:'A:',
          speech:'No. I don’t have any plans.'
        },
        {
          name:'B:',
          speech:'Well, I was wondering if you’d like to go to a movie.'
        },
        {
          name:'A:',
          speech:'Sure. What kind of movie is it?'
        },
        {
          name:'B:',
          speech:'Well, we could see The Blown Identity. It’s a thriller with Mark Diamond.'
        },
        {
          name:'A:',
          speech:'That sounds good. What time does the show start?'
        },
        {
          name:'B:',
          speech:'Eight o’clock. I’ll pick you up at seven.'
        },
        {
          name:'A:',
          speech:'Okay. See you Friday night.'
        },
        ],

        moviedialogs:[
        {
          name:'B:',
          speech:'So, what did you think of the movie?'
        },
        {
          name:'A:',
          speech:'It was hilarious. I think the best part was when James realized his abilities. Like when he started to speak German and fight the policemen.'
        },
        {
          name:'B:',
          speech:'Yeah, that was pretty cool. The only thing I didn’t like was when he fell from the stairs and just walked away.'
        },
        {
          name:'A:',
          speech:'Yeah, that was quite unrealistic.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'안녕하세요.'
        },
        {
          name:'B:',
          speech:'안녕하세요, Linda. Joe입니다.'
        },
        {
          name:'A:',
          speech:'Joe! 잘 지냈어요?'
        },
        {
          name:'B:',
          speech:'좋아요. 금요일 밤에 뭐 할 거예요?'
        },
        {
          name:'A:',
          speech:'아니요. 아무 계획도 없어요.'
        },
        {
          name:'B:',
          speech:'음, 영화 보러 가실래요?'
        },
        {
          name:'A:',
          speech:'물론이죠. 그것은 어떤 종류의 영화에요?'
        },
        {
          name:'B:',
          speech:'음, 우리는 "The Blowed Identity"를 볼 수 있었어요. Mark Diamond와 함께한 스릴러입니다.'
        },
        {
          name:'A:',
          speech:'그거 좋은데요. 언제 시작되죠?'
        },
        {
          name:'B:',
          speech:'8시에요. 7시에 데리러 갈게요.'
        },
        {
          name:'A:',
          speech:'알겠어요. 금요일 밤에 만나요.'
        },
        ],

        movietranslations:[
        {
          name:'B:',
          speech:'그래서, 그 영화에 대해 어떻게 생각했어요?'
        },
        {
          name:'A:',
          speech:'정말 재미있었어요. James 가 능력을 깨달았을 때가 가장 좋았던 것 같아요. 독일어로 말하고 경찰들과 싸우기 시작했을 때처럼요'
        },
        {
          name:'B:',
          speech:'네, 꽤 멋졌어요. 내가 유일하게 싫어하는 것은 그가 계단에서 떨어져 그냥 걸어갔을 때였어요.'
        },
        {
          name:'A:',
          speech:'네, 그건 꽤 비현실적이었어요.'
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
