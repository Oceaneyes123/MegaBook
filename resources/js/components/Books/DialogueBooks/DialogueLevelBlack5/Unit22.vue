<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/hands-holding-house-keys-contract-outdoors_23-2148301719.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Changes
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Changes</li><br />
      <br />
      <p>
        Taking up computer programming
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="enrolldialog in enrolldialogs" :key="enrolldialog">
          <td class = "uppertable" >{{enrolldialog.name}}</td>
          <td class = "lowertable" >{{enrolldialog.speech}}</td>
        </tr>
  
      </table>

      <br />
      <p>
        Renting a room
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="rentdialog in rentdialogs" :key="rentdialog">
          <td class = "uppertable" >{{rentdialog.name}}</td>
          <td class = "lowertable" >{{rentdialog.speech}}</td>
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
            Do you think Robbie will be able to find a job after the course?<br />
          </li>
          <li>
            Is it easy to find a job in Korea? Were you able/Will you be able to find a good job?<br />
          </li>
          <li>
            Do you think Lois will be able to work in her new room?<br />
          </li>
          <li>
            Is your room quiet? Were you able to sleep well yesterday?<br />
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
        <p>
          컴퓨터 프로그래밍 배우기
        </p>
        <br />
        <table style = "border-collapse: collapse;">

          <tr v-for="enrolltranslation in enrolltranslations" :key="enrolltranslation">
            <td class = "uppertable" >{{enrolltranslation.name}}</td>
            <td class = "lowertable" >{{enrolltranslation.speech}}</td>
          </tr>
  
        </table>
        <br />
        <p>
          방 빌리기
        </p>
        <br />
        <table style = "border-collapse: collapse;">

          <tr v-for="renttranslation in renttranslations" :key="renttranslation">
            <td class = "uppertable" >{{renttranslation.name}}</td>
            <td class = "lowertable" >{{renttranslation.speech}}</td>
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
                      동사 can : 미래의 능력은 'will be able to'로 나타냅니다. 조동사 will과 can은 연달아 같이 쓸 수 없기 때문에 can 대신 be able to를 씁니다.<br />
                          Example: <br />
                              I haven't been able to find another one : 다른 사람을 찾을 수 없었습니다 <br />
                              My girlfriend will be able to help me : 내 여자친구가 나를 도와줄 수 있을 것입니다 <br />
                              Will I be able to find a job as a computer programmer? : 컴퓨터 프로그래머 같은 직업을 찾을 수 있을까요?<br /> 
                              You'll be able to get a good job and make lots of money : 당신은 좋은 직장을 얻고 많은 돈을 벌 수 있을 것입니다<br /> 
                              You'll be able to work with no problem : 아무런 문제없이 일 할 수 있을 것입니다 <br />
                              Will I be able to use the kitchen? : 부엌을 사용할 수 있을까요?<br />
                    </li>
                    <li>
                      work on : ~에 종사하다
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
        enrolldialogs:[
        {
          name:'Principal:',
          speech:'Why do you want to study computer programming?'
        },
        {
          name:'Robbie:',
          speech:'Well, I lost my job last month, and I haven’t been able to find another one.'
        },
        {
          name:'Principal:',
          speech:'I see. Do you have any money?'
        },
        {
          name:'Robbie:',
          speech:'Well, some, and my girlfriend will be able to help me.'
        },
        {
          name:'Principal:',
          speech:'Good. The course costs $2,500.'
        },
        {
          name:'Robbie:',
          speech:'Whew! Will I be able to find a job as a computer programmer?'
        },
        {
          name:'Principal:',
          speech:'Oh, sure! You’ll be able to get a good job and make lots of money.... Please sign here.'
        },
        ],

        rentdialogs:[
        {
          name:'Mrs. Wood:',
          speech:'This is the room. Do you like it?'
        },
        {
          name:'Lois:',
          speech:'It’s very nice. Is it quiet? I’m a writer.'
        },
        {
          name:'Mrs. Wood:',
          speech:'You’ll be able to work with no problem. There’s almost no noise here.'
        },
        {
          name:'Lois:',
          speech:'Will I be able to use the kitchen?'
        },
        {
          name:'Mrs. Wood:',
          speech:'Yes, of course.'
        },
        {
          name:'Lois:',
          speech:'Fine. It looks good. (Crash!) What’s that?'
        },
        {
          name:'Mrs. Wood:',
          speech:'Oh, that’s just our neighbor. He works on old cars. (Crash!) He’s usually quiet'
        },
        ],

        enrolltranslations:[
        {
          name:'원장:',
          speech:'Why do you want to study computer programming?'
        },
        {
          name:'Robbie:',
          speech:'Well, I lost my job last month, and I haven’t been able to find another one.'
        },
        {
          name:'원장:',
          speech:'I see. Do you have any money?'
        },
        {
          name:'Robbie:',
          speech:'Well, some, and my girlfriend will be able to help me.'
        },
        {
          name:'원장:',
          speech:'Good. The course costs $2,500.'
        },
        {
          name:'Robbie:',
          speech:'Whew! Will I be able to find a job as a computer programmer?'
        },
        {
          name:'원장:',
          speech:'Oh, sure! You’ll be able to get a good job and make lots of money.... Please sign here.'
        },
        ],

        renttranslations:[
        {
          name:'Wood부인입니다:',
          speech:'여기가 그 방입니다. 마음에 드세요?'
        },
        {
          name:'Lois:',
          speech:'아주 좋아요. 조용해요? 저는 작가입니다.'
        },
        {
          name:'Wood부인:',
          speech:'아무 문제 없이 일할 수 있을 거예요. 여기는 거의 소음이 없어요.'
        },
        {
          name:'Lois:',
          speech:'주방을 쓸 수 있을까요?'
        },
        {
          name:'Wood부인:',
          speech:'네, 물론이죠.'
        },
        {
          name:'Lois:',
          speech:'좋아요. 보기 좋아요. (굉음) 그게 뭐죠?'
        },
        {
          name:'Wood부인:',
          speech:'아, 그건 우리 이웃에 불과해요. 그는 오래된 자동차에서 일합니다. (굉음) 그 사람은 평소에는 말이 없어요.'
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
