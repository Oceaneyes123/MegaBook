<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/young-female-candidate-interviewed-by-employer_1153-3932.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Job interview
        </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Job interview</li><br />

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
            Have you ever had a job interview?<br />
          </li>
          <li>
            What are your strong points?<br />
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
                      want to be : 되기를 원하다<br />
                    </li>
                    <li>
                      work as a(an) 명사 : ~로써 일하다<br />
                    </li>
                    <li>
                      look over : 훑어보다
                    </li>
                    <li>
                      in a few days : 며칠 내에
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
          speech:'Good morning, Miss Benton.'
        },
        {
          name:'B:',
          speech:'Good morning.'
        },
        {
          name:'A:',
          speech:'So you want to be a tour manager?'
        },
        {
          name:'B:',
          speech:'That’s right.'
        },
        {
          name:'A:',
          speech:'Have you ever worked in the travel business?'
        },
        {
          name:'B:',
          speech:'No, but I’ve traveled to a lot of foreign countries. And I speak three languages.'
        },
        {
          name:'A:',
          speech:'That’s good. What kind of work experience do you have?'
        },
        {
          name:'B:',
          speech:'Right now I’m working at the Regal Hotel as a receptionist. Before that, I was a waitress at the Magnolia Restaurant.'
        },
        {
          name:'A:',
          speech:'Tell me more about yourself, Miss Benton. What are your strong points?'
        },
        {
          name:'B:',
          speech:'Well, I’m friendly. I like people. And I’m a hard worker.'
        },
        {
          name:'A:',
          speech:'Why do you want to work for this company?'
        },
        {
          name:'B:',
          speech:'Sunshine Travel has a very good reputation. You’re the best travel agency in town.'
        },
        {
          name:'A:',
          speech:'Thank you. Do you have any questions, Miss Benton?'
        },
        {
          name:'B:',
          speech:'Yes, how much is the starting salary?'
        },
        {
          name:'A:',
          speech:'Two thousand dollars a month, plus living expenses.'
        },
        {
          name:'B:',
          speech:'That sounds good.'
        },
        {
          name:'A:',
          speech:'Yes, it’s a good job. I’ll look over your application and call you in a few days.'
        },
        {
          name:'B:',
          speech:'Thank you.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'좋은 아침이에요, Benton 양.'
        },
        {
          name:'B:',
          speech:'좋은 아침이에요.'
        },
        {
          name:'A:',
          speech:'그래서 관광 매니저가 되고 싶어요?'
        },
        {
          name:'B:',
          speech:'맞아요.'
        },
        {
          name:'A:',
          speech:'여행업계에서 일해 본 적 있어요?'
        },
        {
          name:'B:',
          speech:'아니요, 하지만 외국을 많이 여행했습니다. 그리고 저는 3개 국어를 구사합니다.'
        },
        {
          name:'A:',
          speech:'잘됐네요. 당신은 어떤 종류의 업무 경험을 가지고 있나요?'
        },
        {
          name:'B:',
          speech:'지금은 리갈 호텔에서 접수원으로 일하고 있습니다. 그전에는 매그놀리아 레스토랑의 웨이트리스였습니다.'
        },
        {
          name:'A:',
          speech:'Benton양, 당신에 대해 더 자세히 말해 주세요. 당신의 장점은 무엇입니까?'
        },
        {
          name:'B:',
          speech:'음, 저는 친절합니다. 저는 사람을 좋아합니다. 그리고 저는 열심히 일합니다.'
        },
        {
          name:'A:',
          speech:'왜 이 회사에서 일하고 싶어요?'
        },
        {
          name:'B:',
          speech:'선샤인 트래블은 평판이 아주 좋기 때문입니다. 이 동네 최고의 여행사예요.'
        },
        {
          name:'A:',
          speech:'감사합니다. 궁금한 거 있어요, Benton양?'
        },
        {
          name:'B:',
          speech:'네, 초봉은 얼마예요?'
        },
        {
          name:'A:',
          speech:'매달 2천 달러와 생활비를 더해서요.'
        },
        {
          name:'B:',
          speech:'그거 좋은데요.'
        },
        {
          name:'A:',
          speech:'네, 좋은 직업이에요. 신청서를 검토해 보고 며칠 후에 전화할게요.'
        },
        {
          name:'B:',
          speech:'감사합니다.'
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
