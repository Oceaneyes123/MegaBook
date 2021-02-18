<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/headlines_1101-727.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Looking for a job
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Looking for a job</li><br />

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
          <u>Look at the two ads, and have a similar conversation as the two persons above. Make a phone call to apply for one of the following jobs; ask about qualifications and salary.</u><br />
        </p>

        <v-container grid-list-md text-xs-center>
          <v-layout wrap align-content-center>

            <v-flex xs12 md4 >
              <v-card hover>

                <v-img src="images/kfcmap.gif" />

              </v-card>
            </v-flex>

          </v-layout>
        </v-container>

        <p>
          PT = part time<br />
          FT = full time<br />
          min. 2 yrs. exp. = minimum two years’ experience<br />
          local ref. = local references (people who recommend you for the job live in this area)<br />
          $8.00/hr. = eight dollars an hour<br />
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
                      현재분사 : 형태는 동사원형+ing 이고 명사를 수식하는 경우 능동 혹은 진행의 의미로 ~하는, ~하고 있는 으로 해석합니다.  be동사와 함께 쓰이면 진행형이 됩니다.<br />
                          Ex: It's a job selling encyclopedias (그것은 사전을 파는 직업입니다<br />
                    </li>
                    <li>
                      someone with experience : 경험이 있는 사람<br />
                    </li>
                    <li>
                      why don't you : ~하는 게 어때? = what about, how about
                    </li>
                    <li>
                      give a call : 전하다
                    </li>
                    <li>
                      experience in : ~에서의 경험
                    </li>
                    <li>
                      good with people : 사람들과 잘 지내다
                    </li>
                    <li>
                      at least : 최소한, 적어도
                    </li>
                    <li>
                      apply for : ~을 위해 적용하다, 신청하다
                    </li>
                    <li>
                      make an appointment : 약속을 정하다
                    </li>
                    <li>
                      where are you located? : 위치가 어디입니까?
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
          speech:'Are there any interesting jobs in the paper today?'
        },
        {
          name:'B:',
          speech:'Here’s one for a salesperson. It’s a job selling encyclopedias.'
        },
        {
          name:'A:',
          speech:'What’s the salary?'
        },
        {
          name:'B:',
          speech:'I think it’s commission only.'
        },
        {
          name:'A:',
          speech:'That’s no good.'
        },
        {
          name:'B:',
          speech:'There’s another one here for a tour guide.'
        },
        {
          name:'A:',
          speech:'Do they want someone with experience?'
        },
        {
          name:'B:',
          speech:'It doesn’t say.'
        },
        {
          name:'A:',
          speech:'Why don’t you give them a call?'
        },
        {
          name:'B:',
          speech:'I think I will.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'Sunshine Travel. May I help you?'
        },
        {
          name:'B:',
          speech:'I’m calling about the job for a tour guide. Is it still open?'
        },
        {
          name:'C:',
          speech:'Yes, it is.'
        },
        {
          name:'B:',
          speech:'What are the qualifications?'
        },
        {
          name:'C:',
          speech:'We’re looking for someone with experience in the travel business. You must be good with people and speak at least one foreign language.'
        },
        {
          name:'B:',
          speech:'How can I apply for the job?'
        },
        {
          name:'C:',
          speech:'You have to come in, get an application and make an appointment for an interview.'
        },
        {
          name:'B:',
          speech:'Where are you located?'
        },
        {
          name:'C:',
          speech:'537 Lime Street, downtown.'
        },
        {
          name:'B:',
          speech:'Thank you. I’ll come tomorrow.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'오늘 신문에 재미있는 일이 있나요?'
        },
        {
          name:'B:',
          speech:'여기 영업사원 한 명 있어요. 백과사전을 파는 직업입니다.'
        },
        {
          name:'A:',
          speech:'월급이 얼마예요?'
        },
        {
          name:'B:',
          speech:'수수료만 주는 것 같아요.'
        },
        {
          name:'A:',
          speech:'그건 좋지 않아요.'
        },
        {
          name:'B:',
          speech:'여기 관광 안내원이 하나 더 있어요.'
        },
        {
          name:'A:',
          speech:'그들은 경험이 있는 사람을 원하나요?'
        },
        {
          name:'B:',
          speech:'그건 안 나와요.'
        },
        {
          name:'A:',
          speech:'그들에게 전화하는 게 어때요?'
        },
        {
          name:'B:',
          speech:'그럴 것 같아요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'선샤인 트래블입니다. 무엇을 도와드릴까요?'
        },
        {
          name:'B:',
          speech:'관광 안내원 일자리 때문에 전화드렸습니다. 아직도 열려 있나요?'
        },
        {
          name:'C:',
          speech:'네, 그렇습니다.'
        },
        {
          name:'B:',
          speech:'자격 요건이 뭐죠?'
        },
        {
          name:'C:',
          speech:'저희는 여행업에 경험이 있는 사람을 찾고 있습니다. 당신은 사람들과 잘 어울리고 적어도 한 가지 외국어를 할 줄 알아야 합니다.'
        },
        {
          name:'B:',
          speech:'그 일자리에 지원하려면 어떻게 해야 하나요?'
        },
        {
          name:'C:',
          speech:'들어오셔서 원서를 받고 면접 약속을 잡으셔야 합니다.'
        },
        {
          name:'B:',
          speech:'어디에 있어요?'
        },
        {
          name:'C:',
          speech:'시내에 있는 라임 가 537번지입니다.'
        },
        {
          name:'B:',
          speech:'감사합니다. 내일 올게요'
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
