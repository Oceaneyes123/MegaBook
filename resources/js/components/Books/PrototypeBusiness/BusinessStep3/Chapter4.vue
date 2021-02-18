<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGyDSYeX4/4/screen_2x/canva-close-up-photography-of-white-poodle--MADGyDSYeX4.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgba(140, 103, 90, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing work in progress
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color:#402B24; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border white--text" >Today's topic</h3>
  <div style = "padding : 16px;">

    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table> 
    
    
    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #402B24;">Translation</h3>
      <div style="padding : 16px;">

          <table style = "border-collapse: collapse;">

              <tr v-for="translation in translations" :key="translation">
                  <td class = "uppertable" >{{translation.name}}</td>
                  <td class = "lowertable" >{{translation.speech}}</td>
              </tr>

          </table>
      </div>

    
    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Exercise</h3>
      <div style="padding : 16px;">


        <p>
          Answer the questions.
        </p>

        <ol style="margin: 12px;">
          <li>
            Which country is John working in?
          </li>
          <li>
            What’s the project?
          </li>
          <li>
            What’s the budget for the project?
          </li>
          <li>
            How much of the work is John paying for?
          </li>
          <li>
            How long is the schedule?
          </li>
        </ol>

        <p>
           Free response:<br />
           Talk about a project or job you're working on at the moment. How's it going?
        </p>

      </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Self Study</h3>
      <div style="padding : 16px;">


          <p>
            Notes
          </p>

        <p>

          <v-container grid-list-md text-xs-left>
            <v-layout row wrap>


              <v-flex xs12>
                <v-card light color="#F2CBBD">
                  <v-card-text class="px-10">
                <p>
                  Present continuous
                </p>
                <p>
                  Where <b>are you</b> working at the moment?<br />
                  <b>I’m working</b> in Italy.<br />
                  <b>Is</b> Kathy <b>working</b> with you?<br />
                  She <b>isn’t working</b> on this project. or She’s not working on this project.
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
          name:'Vanessa:',
          speech:'So where are you working? exactly in France?'
        },
        {
          name:'John:',
          speech:'In the Jura. It’s not far from Switzerland.'
        },
        {
          name:'Vanessa:',
          speech:'Right. And you’re building a hotel?'
        },
        {
          name:'John:',
          speech:'We’re converting a farmhouse into a hotel. It’s very, um…it’s a very old house. When we started, it had no windows, no doors…it was a ruin, basically.'
        },
        {
          name:'Vanessa:',
          speech:'And now?'
        },
        {
          name:'John:',
          speech:'Well, now. Most of the work’s complete. I’m staying in one of the rooms, in fact, so, um, I’m the first guest.'
        },
        {
          name:'Vanessa:',
          speech:'You’re the boss, though, so you’re not paying.'
        },
        {
          name:'John:',
          speech:'Oh, I’m paying! This project’s costing a fortune!'
        },
        {
          name:'Vanessa:',
          speech:'I see. Well, that’s one of my questions, actually. What’s your budget?'
        },
        {
          name:'John:',
          speech:'Um…the total budget’s five hundred and sixty thousand euros…and I’m paying half of that. Richard and Kathy Mills are paying the rest. They’re my business partners.'
        },
        {
          name:'Vanessa:',
          speech:'And your business partners are hotel managers, Is that right?'
        },
        {
          name:'John:',
          speech:'That’s right. I’m managing the project ? the construction. And they’re still living and working in the UK at the moment, organizing the website and the marketing material, you know, brochures and things. Then they plan to live here and manage the hotel when it’s finished.'
        },
        {
          name:'Vanessa:',
          speech:'I see. So, how long are you staying in France? What’s the schedule, from start to finish?'
        },
        {
          name:'John:',
          speech:'Um…Eighteen months. And we’re more or less on schedule. At the moment, we’re working on the bathroom. We’re having one or two problems with…'
        },
        ],

        translations:[
        {
          name:'바네사:',
          speech:'그럼 어디서 일해요? 바로 그거에요 프랑스에서요?'
        },
        {
          name:'존:',
          speech:'주라에서요. 스위스에서 멀지 않아요.'
        },
        {
          name:'바네사:',
          speech:'맞아요. 그리고 당신은 호텔을 짓고 있나요?'
        },
        {
          name:'존:',
          speech:'우리는 농가를 호텔로 개조하고 있어요. 아주, 음... 아주 오래된 집이에요. 우리가 시작했을 때, 창문도, 문도 없었습니다. 기본적으로 그것은 폐허가 되었습니다.'
        },
        {
          name:'바네사:',
          speech:'그러면 지금은?'
        },
        {
          name:'존:',
          speech:'자, 이제요. 대부분의 작업이 완료되었습니다. 실은 제가 첫 손님이라서요.'
        },
        {
          name:'바네사:',
          speech:'그래도 사장님이시니까 계산은 안 하시는군요.'
        },
        {
          name:'존:',
          speech:'아, 저는 돈을 냅니다! 이 프로젝트는 엄청난 비용이 듭니다!'
        },
        {
          name:'바네사:',
          speech:'그렇군요, 사실 그게 제 질문 중 하나죠 예산이 어떻게 되세요?'
        },
        {
          name:'존:',
          speech:'음... 총 예산은 56만 유로이고, 그 절반은 제가 부담하고 있어요. 리차드와 캐시 밀스가 나머지를 지불하고 있습니다. 그들은 제 사업 파트너입니다.'
        },
        {
          name:'바네사:',
          speech:'그리고 당신의 사업 파트너는 호텔 매니저인데, 맞나요?'
        },
        {
          name:'존:',
          speech:'맞아요. 저는 그 프로젝트를 관리하고 있습니다. 그리고 그들은 여전히 영국에서 일하고 있습니다. 웹사이트와 마케팅 자료를 정리하면서 말이죠. 브로슈어 같은 것들 말입니다. 그리고나서 그들은 여기서 살면서 호텔이 완성되면 관리해 줄 계획입니다.'
        },
        {
          name:'바네사:',
          speech:'그렇군요. 그럼 프랑스에는 얼마나 머무르실 건가요? 스케줄이 어떻게 되나요, 처음부터 끝까지?'
        },
        {
          name:'존:',
          speech:'음…18개월입니다. 그리고 우리는 어느 정도 일정에 맞추어져 있습니다. 지금은 화장실 작업을 하고 있습니다. 하나 또는 두 가지 문제가 있습니다.'
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
  border-color: transparent#402B24 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background:#402B24;
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

