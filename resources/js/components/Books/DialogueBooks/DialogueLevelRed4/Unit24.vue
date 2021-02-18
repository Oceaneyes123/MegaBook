<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/young-traveler-talking-smartphone-airport_1163-3263.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Elmer calls home
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br />( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Elmer calls home</li><br />
      <br />
      <p>
        Elmer Colt is from Kansas. He's on a 14-day tour of Europe. The tour started in London. At the moment he's in Prague. It's the eighth day of the tour. He's already been to eight countries and stayed in the principal cities. He's never been to Europe before. Elmer calls home.<br />
      </p>
      <br />
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
            What countries have you visited?
          </li>
          <li>
            Would you like to visit Europe?
          </li>
          <li>
            What countries would you like to visit?
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
          Elmer Colt는 캔자스 출신입니다. 그는 14일 동안 유럽 여행을 하고 있어요. 투어는 런던에서 시작되었습니다. 지금 그는 프라하에 있습니다. 투어 8일째입니다. 그는 이미 8개국을 다녀왔고 주요 도시에 머물렀습니다. 그는 전에 유럽에 가본 적이 없어요. Elmer가 집에 전화해요.<br />
        </p>
        <br />
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
                      현재완료의 경험 : 과거에서 현재까지의 기간 동안에 있었던 일을 나타낼 때 쓰입니다. <br />
                      '~한 적이 있다'라고 해석하며, 사건이 일어난 때를 정확히 알 수 없거나 굳이 밝힐 필요가 없을 때 씁니다. ever, never, before 등과 함께 자주 쓰입니다.<br />                  
                    </li>
                    <li>
                      have been to + 장소 :~에 간 적이 있다(경험), ~에 갔다 왔다(완료)<br />
                    </li>
                    <li>
                      have gone to + 장소 : ~ 갔다(완료, 가서 지금 이 자리에 없는 경우)
                    </li>
                    <li>
                      at the moment : 지금 바로, 현재, 바로 지금
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
          name:'Elmer:',
          speech:'Hello, Mom? Is that you?'
        },
        {
          name:'Mrs. Colt:',
          speech:'Oh, Elmer, yes. How are you? Where are you now?'
        },
        {
          name:'Elmer:',
          speech:'I’m fine. I’ve just arrived in Prague, Mom.'
        },
        {
          name:'Mrs. Colt:',
          speech:'You haven’t sent us any postcards yet.'
        },
        {
          name:'Elmer:',
          speech:'Yes, I have. I’ve sent one from every city.'
        },
        {
          name:'Mrs. Colt:',
          speech:'Have you been to Paris yet, Elmer?'
        },
        {
          name:'Elmer:',
          speech:'Yes, I have.'
        },
        {
          name:'Mrs. Colt:',
          speech:'Have you been to Vienna yet?'
        },
        {
          name:'Elmer:',
          speech:'No, I haven’t. We’re going to Vienna tomorrow.'
        },
        {
          name:'Mrs. Colt:',
          speech:'How many countries have you seen now?'
        },
        {
          name:'Elmer:',
          speech:'Well, this is the eighth day, so I’ve already seen eight countries.'
        },
        {
          name:'Mrs. Colt:',
          speech:'Have you spent much money?'
        },
        {
          name:'Elmer:',
          speech:'Well, uh, yes, Mom. I’ve bought a lot of souvenirs, and I want to buy some more. Can you send me a thousand dollars?'
        },
        {
          name:'Mrs. Colt:',
          speech:'All right, Elmer. And have you taken many pictures?'
        },
        {
          name:'Elmer:',
          speech:'Yes, I’ve taken a lot. I’ve used three rolls of film!'
        },
        {
          name:'Mrs. Colt:',
          speech:'Have you met any nice girls yet?'
        },
        {
          name:'Elmer:',
          speech:'Oh, yes, Mom. There’s a girl from Texas on the tour. We’ve done everything together.'
        },
        ],

        translations:[
        {
          name:'Elmer:',
          speech:'여보세요? 엄마에요?'
        },
        {
          name:'Colt 부인:',
          speech:'아, Elmer, 그래. 잘 지내? 지금 어디에 있어?'
        },
        {
          name:'Elmer:',
          speech:'전 괜찮아요. 엄마, 나 방금 프라하에 도착했어요.'
        },
        {
          name:'Colt 부인:',
          speech:'아직 우리에게 엽서를 보내지 않았어.'
        },
        {
          name:'Elmer:',
          speech:'모든 도시에서 하나를 보냈어요.'
        },
        {
          name:'Colt 부인:',
          speech:'Elmer, 파리에 가본 적 있어?'
        },
        {
          name:'Elmer:',
          speech:'네.'
        },
        {
          name:'Colt 부인:',
          speech:'비엔나에 가 봤어?'
        },
        {
          name:'Elmer:',
          speech:'아니요, 안 봤어요. 내일 비엔나에 가요.'
        },
        {
          name:'Colt 부인:',
          speech:'지금 몇 개국을 가봤어?'
        },
        {
          name:'Elmer:',
          speech:'음, 오늘이 여덟 번째 날이에요. 그래서 저는 벌써 여덟 나라를 봤어요.'
        },
        {
          name:'Colt 부인:',
          speech:'돈을 많이 썼어?'
        },
        {
          name:'Elmer:',
          speech:'음, 어, 네, 엄마. 기념품을 많이 샀는데, 좀 더 사고 싶어요.  1,000달러만 보내줄래요?'
        },
        {
          name:'Colt 부인:',
          speech:'좋아, Elmer. 그리고 사진은 많이 찍었어?'
        },
        {
          name:'Elmer:',
          speech:'네, 많이 찍었어요. 필름을 세 통이나 썼어요!'
        },
        {
          name:'Colt 부인:',
          speech:'좋은 여자 만나 봤어?'
        },
        {
          name:'Elmer:',
          speech:'아, 네, 엄마. 텍사스 출신의 한 소녀가 투어에 참가하고 있어요. 우리는 모든 것을 함께 했어요.'
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
