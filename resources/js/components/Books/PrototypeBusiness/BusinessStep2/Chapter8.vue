<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADQ5tITPus/1/screen_2x/canva-people-at-a-cafe-MADQ5tITPus.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Talking about the weather and climate 2
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
        Answer the questions.
      </p>

      <p>
        - What's the weather like today?<br />
        - What city are the colleagues in?<br />
        - What's the Mistral?<br />
        - What's the weather like in London today?<br />
        Free response:<br />
        Talk about your past experiences of extreme weather:<br />
        - very hot weather<br />
        - very cold weather<br />
        - heavy snow<br />
        - heavy rain<br />
        - strong winds
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
                    The climate
                  </p>
                  <p>
                    It rains a lot in the UK in April.<br />
                    It's open foggy in November.<br />
                  </p>
                  <p>
                    The weather now<br />
                    It's freezing.<br />
                    It's snowing.
                  </p>
                  <p>
                    The weather in the past<br />
                    It rained last night.<br />
                    It was windy yesterday.
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
          name:'Nigel:',
          speech:' Well, it’s a beautiful day.'
        },
        {
          name:'Olivier:',
          speech:'Yeah, it’s nice to see the sun. It rained nearly every day last week.'
        },
        {
          name:'Nigel:',
          speech:'Really?'
        },
        {
          name:'Olivier:',
          speech:'Yeah. Not a very good start to the summer.'
        },
        {
          name:'Nigel:',
          speech:'Does it normally rain much here, in July?'
        },
        {
          name:'Olivier:',
          speech:'No. You sometimes get one or two wet days. Or thunderstorms, sometimes. But, um... anyway, the sun’s shining today, that’s the main thing.'
        },
        {
          name:'Nigel:',
          speech:'Yes. Ah... The waiter’s coming with our bottle of water.'
        },
        {
          name:'Olivier:',
          speech:'Thank you. Would you like some?'
        },
        {
          name:'Nigel:',
          speech:'Yes, please.'
        },
        {
          name:'Olivier:',
          speech:'So, is this your first visit to Marseille?'
        },
        {
          name:'Nigel:',
          speech:' No. I came here once before, about two years ago. In winter. It was... It was quite warm, actually.'
        },
        {
          name:'Olivier:',
          speech:'Yeah, winter is great here. Before, when I lived in Paris, I always hated winter. But here, it’s, um... If there’s no wind, and the sun’s out, you can wear a T-shirt. We get a cold wind, sometimes, called the Mistral. It blows down from the mountains... from the Alps. But, um... if it’s sunny, and there’s no wind, then it’s... it’s quite warm.'
        },
        {
          name:'Nigel:',
          speech:'Well, my boss phoned me, from the UK office, half an hour ago. Apparently, it’s raining there at the moment..'
        },
        {
          name:'Olivier:',
          speech:'Oh dear.'
        },
        {
          name:'Nigel:',
          speech:'So, here’s to our colleagues in London!'
        },
        {
          name:'Olivier:',
          speech:'Yes. Cheers!'
        },
        {
          name:'Nigel:',
          speech:'Cheers!'
        },
        ],

        translations:[
        {
          name:'나이젤:',
          speech:' 음, 아름다운 날이야.'
        },
        {
          name:'올리비에:',
          speech:'그래, 햇빛을 보니 좋구나. 지난주에는 거의 매일 비가 왔어.'
        },
        {
          name:'나이젤:',
          speech:'그래?'
        },
        {
          name:'올리비에:',
          speech:'그래, 여름의 시작은 별로 좋지 않아.'
        },
        {
          name:'나이젤:',
          speech:'여기는 보통 7월에 비가 많이 오니?'
        },
        {
          name:'올리비에:',
          speech:'아니. 가끔 한두 날이 비 오는 경우도 있다. 천둥 번개를 동반한 폭풍우이기도 해. 하지만, 음... 어쨌든, 오늘은 태양이 빛나고 있어, 그게 중요한 거야.'
        },
        {
          name:'나이젤:',
          speech:'응. 아... 웨이터가 우리 물병을 가지고 오고 있어.'
        },
        {
          name:'올리비에:',
          speech:'고마워 뭐 좀 먹을래?'
        },
        {
          name:'나이젤l:',
          speech:'응.'
        },
        {
          name:'올리비에:',
          speech:'그래, 마르세유에 처음 방문하는 거야?'
        },
        {
          name:'나이젤:',
          speech:'아니야. 여기 한 번 온 적이 있는데, 2년 전쯤이야. 겨울에. 그건... 사실 꽤 따뜻했어.'
        },
        {
          name:'올리비에:',
          speech:'그래, 여기 겨울은 대단해. 예전에 내가 파리에 살 때, 나는 항상 겨울이 싫었어. 하지만 여기선, 음... 바람이 없고 해가 지면 티셔츠를 입을 수 있어. 우리는 가끔 미스트랄이라 불리는 찬바람을 맞기도 해. 산에서 불어 내려와.. 알프스 산맥에서 하지만, 음... 해가 쨍쨍하고 바람이 없으면... 꽤 따뜻해.'
        },
        {
          name:'나이젤:',
          speech:'음, 내 상사가 30분 전에 영국 사무실에서 나에게 전화를 했어. 보아하니, 지금 거기는 비가 오고 있대.'
        },
        {
          name:'올리비에:',
          speech:'맙소사.'
        },
        {
          name:'나이젤:',
          speech:'자, 런던에 있는 우리 동료들을 위해 건배!'
        },
        {
          name:'올리비에:',
          speech:'그래. 건배!'
        },
        {
          name:'나이젤:',
          speech:'건배!'
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
