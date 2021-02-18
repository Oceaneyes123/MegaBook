<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/young-it-service-man-repairing-computer_1303-19460.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Giving an update
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
          Fill in the gaps with already, yet or so far.
        </p>

        <ol style="margin: 12px;">
          <li>
            Have you finished <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; </u>?
          </li>
          <li>
            We have to build six units today, and we've only built two <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; </u>.
          </li>
          <li>
             I didn't plan to finish all the work today, but I've <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; </u> done everything.
          </li>
          <li>
            The work has gone well <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; </u>, but we haven't done the hardest job <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; </u>.
          </li>
        </ol>

        <p>
          Free response:<br />
          Discuss air travel.<br />
          Which airlines do you use?<br />
          Which is your favorite airline?<br />
          Do you often fly long distances?<br />
          Do you like travelling by plane? Why/Why not?
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
                Present perfect: yet/already/so far<br />
                Have you written that report <b>yet</b>?<br />
                I’ve started it, but I haven’t finished it <b>yet</b>.<br />
                We’re doing well. We’ve <b>already</b> done most of the work.<br />
                I’m reading your report. I’ve read half of it <b>so far</b>.
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
          name:'Yves:',
          speech:'Yves Cordier.'
        },
        {
          name:'Andy:',
          speech:'Yves, it’s Andy Bell.'
        },
        {
          name:'Yves:',
          speech:'Andy, hi, how are things?'
        },
        {
          name:'Andy:',
          speech:'Going quite well.'
        },
        {
          name:'Yves:',
          speech:'Is everything nearly ready?'
        },
        {
          name:'Andy:',
          speech:'Well, we’ve got a full accounts department. I interviewed someone on Monday and she’s accepted the post. Sara Bernard. I’ve already sent her details to personnel, so that’s gone well…'
        },
        {
          name:'Yves:',
          speech:'OK, good. And, what about the IT system? Have they installed that yet?'
        },
        {
          name:'Andy:',
          speech:'Well, that’s more difficult. Um… I’ve found two technicians so far, er, but unfortunately, I haven’t found the third person we need, so…'
        },
        {
          name:'Yves:',
          speech:'So you haven’t finished the IT installation?'
        },
        {
          name:'Andy:',
          speech:'No, we… we haven’t actually started it yet. But…'
        },
        {
          name:'Yves:',
          speech:'You haven’t started it yet? Andy, we need to open that office in two weeks!'
        },
        {
          name:'Andy',
          speech:'I know. I’ve spoken to Daniela in the Zurich office and she’s going to send someone next week. I think we can still open on time.'
        },
        {
          name:'Yves',
          speech:'We need to. How long is it going to take for you to get…'
        },
         ],
      
      translations:[
      {
          name:'이브:',
          speech:'이브 코디어 입니다.'
        },
        {
          name:'앤디:',
          speech:'이브, 저 앤디 벨입니다.'
        },
        {
          name:'이브:',
          speech:'앤디, 안녕하세요, 요즘 어때요?'
        },
        {
          name:'앤디:',
          speech:'잘 지내요.'
        },
        {
          name:'이브:',
          speech:'모든 것이 거의 다 준비되었나요?'
        },
        {
          name:'앤디:',
          speech:'음, 우리는 회계 부서가 꽉 찼어요. 내가 월요일에 누군가를 인터뷰했는데 그녀가 그 직책을 수락했어요. 새라 버나드. 저는 이미 그녀의 세부사항을 인사과로 보냈기 때문에, 그것은 잘 되었습니다.'
        },
        {
          name:'이브:',
          speech:'좋아요. 그리고, IT 시스템은 어떤가요? 아직 설치 안 했나요?'
        },
        {
          name:'앤디:',
          speech:'글쎄요, 그게 더 어려워요. 음... 지금까지 두 명의 기술자를 찾았는데 아쉽게도 세 번째 필요한 사람을 찾지 못했어요.'
        },
        {
          name:'이브:',
          speech:'그럼 IT 설치를 완료하지 않으셨습니까?'
        },
        {
          name:'앤디:',
          speech:'네, 우리는 아직 시작도 안 했습니다. 그런데...'
        },
        {
          name:'이브:',
          speech:'아직 시작하지 않았어요? 앤디, 2주 안에 사무실을 열어야 해요!'
        },
        {
          name:'앤디',
          speech:'알아요. 취리히 사무실에 있는 다니엘라와 통화했는데 다음 주에 사람을 보낼 거예요. 아직 제 시간에 문을 열 수 있을 것 같아요.'
        },
        {
          name:'이브',
          speech:'우리는 그래야 해요. 시간이 얼마나 걸릴까요…'
        }

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
