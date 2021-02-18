<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADQ40qcmqo/1/screen/canva-zakynthos-island-in-greece-MADQ40qcmqo.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgba(254, 183, 43, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Talking about holidays
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border" >Today's topic</h3>
  <div style = "padding : 16px;">

    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table>


 <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Translation</h3>
    <div style="padding : 16px;">

      <table style = "border-collapse: collapse;">

        <tr v-for="translation in translations" :key="translation">
          <td class = "uppertable" >{{translation.name}}</td>
          <td class = "lowertable" >{{translation.speech}}</td>
        </tr>

      </table>
  
    </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Exercise</h3>
    <div style="padding : 16px;">

      <p>
        Write the past simple form of the verbs.
      </p>

      <ol style="margin: 12px;">
        <li>
          We  ( &emsp; ) back last night. (fly)
        </li>
        <li>
          I  ( &emsp; ) this CD on my holiday.(buy)
        </li>
        <li>
          IS  ( &emsp; ) home last Friday.(come)
        </li>
        <li>
          We  ( &emsp; ) a ferry to the island. (take)
        </li>
      </ol>

      <p>
        Free response:<br />
        Talk about past holiday with a partner.<br />
        Where/What/How did...?
      </p>

    </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Self Study</h3>
    <div style="padding : 16px;">


      <p>
        Notes
      </p>

      <p>

        <v-container grid-list-md text-xs-left>
          <v-layout row wrap>


            <v-flex xs12>
              <v-card light color="#527318">
                <v-card-text class="px-10">
                  <p>
                    Past simple: irregular verbs
                  </p>
                  <p>
                    be:was/were<br />
                    become/became<br />
                    come/came<br />
                    do/did<br />
                    drive/drove<br />
                    leave/left<br />
                    see/saw<br />
                    send/sent<br />
                    sleep/slept<br />
                    ...
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
          name:'Hanna:',
          speech:'Hi Steven.'
        },
        {
          name:'Steven:',
          speech:'Oh hi, Hanna. How are you?'
        },
        {
          name:'Hanna:',
          speech:'OK thanks. And you?'
        },
        {
          name:'Steven:',
          speech:'Not too bad. The first day back is never easy, but...'
        },
        {
          name:'Hanna:',
          speech:'Oh, of course, you’re just back from holiday. I bet it was quiet in the office last week- I was in India, Martin was in Mexico, you were... where did you go?'
        },
        {
          name:'Steven:',
          speech:'Greece. Crete.'
        },
        {
          name:'Hanna:',
          speech:'Crete, OK. So how was it?'
        },
        {
          name:'Steven:',
          speech:'Fantastic. We really enjoyed it. We had two days in Athens, as well.'
        },
        {
          name:'Hanna:',
          speech:'Right. So your flight was to Athens?'
        },
        {
          name:'Steven:',
          speech:'Yeah. We flew to Athens. We stayed in a hotel there for... just one night. Then we took a ferry to Crete.'
        },
        {
          name:'Hanna:',
          speech:'The ferry left from Athens, then.'
        },
        {
          name:'Steven:',
          speech:'Yeah. It went directly to Chania in Crete, which was the town where we stayed, so...'
        },
        {
          name:'Hanna:',
          speech:'And did you stay in a hotel?'
        },
        {
          name:'Steven:',
          speech:'No, we rented an apartment-nothing special. We didn’t spend a lot of time in it, really. We ate out every night.'+
          ' The nightlife was good-lots of restaurants and bars,and,er... the food was generally good... and it cost very little for a good meal.'
        },
        {
          name:'Hanna:',
          speech:'Mmm. So you enjoyed the food, and drank Greek wine, and...'
        },
        {
          name:'Steven:',
          speech:'Yeah. It was... all very relaxing.'
        },
        {
          name:'Hanna:',
          speech:'And how much of the island did you see? Did you travel around?'
        },
        {
          name:'Steven:',
          speech:'Yeah. We saw quite a few different places.'
        },
        {
          name:'Hanna:',
          speech:'So you rented a car and drove around, then...'
        },
        {
          name:'Steven:',
          speech:'No, no. We... we went on coach trips-organized trips-on a couple of days. And we travelled around by bus as well.'+
          ' You know, on... just on public buses. I don’t speak a word of Greek, but... you just bought your ticket and... it was no problem.'
        },
        {
          name:'Hanna:',
          speech:'Sounds good.'
        },
        {
          name:'Steven:',
          speech:'We came back on Friday. So I had the weekend at home. And now...back to work! So how was your trip?'
        },
        ],

        translations:[
        {
          name:'한나:',
          speech:'안녕하세요. 스티븐.'
        },
        {
          name:'스티븐:',
          speech:'오 안녕하세요, 한나. 잘지내시죠?'
        },
        {
          name:'한나:',
          speech:'네. 스티븐은 어때요?'
        },
        {
          name:'스티븐:',
          speech:'그리 나쁘진 않아요. 돌아오는 첫날은 결코 쉽지 않지만...'
        },
        {
          name:'한나:',
          speech:'아, 물론이죠, 휴가에서 막 돌아왔군요. 지난주에 사무실 안은 조용했겠지죠. 전 인도에 있었고 마틴은 멕시코에 있었고... 당신은 어디 갔었나요?'
        },
        {
          name:'스티븐:',
          speech:'그리스. 크레타요.'
        },
        {
          name:'한나:',
          speech:'크레타, 그렇군요. 그래서 어땠어요?'
        },
        {
          name:'스티븐:',
          speech:'환상 적이에요. 우리는 정말 즐거웠어요. 우리는 아테네에서도 이틀을 보냈어요.'
        },
        {
          name:'한나:',
          speech:'그렇구나. 그럼 당신의 비행기는 아테네로 갔다는 갔나요?'
        },
        {
          name:'스티븐:',
          speech:'네. 우리는 비행기를 타고 아테네로 갔어요. 우리는 그곳에서 단 하루 밤만 호텔에 묵었어요 그리고 크레타행 페리를 탔어요.'
        },
        {
          name:'한나:',
          speech:'그럼 페리는 아테네에서 출발했겠군요.'
        },
        {
          name:'스티븐:',
          speech:'네. 우리가 머물렀던 마을 크레타에 있는 차니아로 직행했으니까...'
        },
        {
          name:'한나:',
          speech:'그리고 호텔에 묵었나요?'
        },
        {
          name:'스티븐:',
          speech:'아니요, 우리는 아파트를 빌렸어.요 특별한 건 없었어요. 우리는 그 안에서 많은 시간을 보내지 않았어요, 정말로. 우리는 매일 밤 외식을 했습니다. 밤에 할 수 있는 오락은 좋았어요. 식당과 술집이 즐비했고... 음식은 대체로 좋았어요... 그리고 좋은 식사에 매우 적은 비용이 들었어요.'
        },
        {
          name:'한나:',
          speech:'음. 그래서 당신은 음식을 맛있게 먹고, 그리스 와인을 마셨고, 그리고...'
        },
        {
          name:'스티븐:',
          speech:'네. 그건... 모두 아주 느긋하게'
        },
        {
          name:'한나:',
          speech:'그리고 섬에서 얼마나 많이 봤나요? 당신은 여기저기 여행했나요?'
        },
        {
          name:'스티븐:',
          speech:'네. 우리는 꽤 많은 다른 장소들을 봤어요.'
        },
        {
          name:'한나:',
          speech:'그러니까 차를 빌려서 돌아다니다가...'
        },
        {
          name:'스티븐:',
          speech:'아니요. 우린 이틀에 걸쳐 코치 여행 계획을 짜서 여행을 떠났어요. 그리고 버스도 타고 돌아다녔어요. 있잖아요, 공공 버스로 말이에요. 그리스어는 한 마디도 못하지만... 단지 표를 샀고... 문제없었어요.'
        },
        {
          name:'한나:',
          speech:'좋았겠네요.'
        },
        {
          name:'스티븐:',
          speech:'우리는 금요일에 돌아왔어요. 그래서 저는 주말을 집에서 보냈어요. 그리고 이제... 다시 일하러 가요! 그래서, 당신의 여행은 어땠어요?'
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
  border-color: transparent #899857 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background: #899857;
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
