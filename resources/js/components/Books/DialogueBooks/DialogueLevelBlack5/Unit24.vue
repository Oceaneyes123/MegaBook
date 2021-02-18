<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/asian-girl-opens-umbrella-rainy-day_46139-1659.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Talking about the weather
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br />( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Talking about the weather</li><br />

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
          <u>Answer the questions, using: I might..</u><br />
          Ex) When will you go to the beach? – I might go tomorrow, if it doesn’t rain.
        </p>
        <br />
        <ol style="margin: 12px;">
          <li>
            What will you do this weekend if the weather’s nice?
          </li>
          <li>
            Will you go swimming this year?
          </li>
          <li>
            When will you go skiing?
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
                      조동사 might : ~일지도 모른다 <br />
                        Example:<br />
                            I might go to the beach later (나는 후에 해변에 갈지도 모른다)<br />
                            It might rain this afternoon (오늘 오후에 비가 올지도 모른다<br />
                            It might stop raining soon (곧 비가 그칠지도 모른다)<br />
                            I think we might have a storm tonight (오늘 폭풍이 있을런지도 모른다고 생각한다)<br />
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
          speech:'Good morning, Libby.'
        },
        {
          name:'B:',
          speech:'Hi, Jake. It’s a nice day, isn’t it?'
        },
        {
          name:'A:',
          speech:'Yeah. What are you doing today?'
        },
        {
          name:'B:',
          speech:'I’m not sure. I might go to the beach later.'
        },
        {
          name:'A:',
          speech:'Well, take an umbrella. I’ve just seen the weather report. It might rain this afternoon'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'A:',
          speech:'Good afternoon, Mrs. Acuna.'
        },
        {
          name:'C:',
          speech:'Hello, Jake. It isn’t very nice today, is it?'
        },
        {
          name:'A:',
          speech:'It was a nice morning. It might stop raining soon.'
        },
        {
          name:'C:',
          speech:'I hope so.'
        },
        {
          name:'A:',
          speech:'Are you playing tennis today?'
        },
        {
          name:'C:',
          speech:'Maybe, it depends on the weather.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'A:',
          speech:'Good evening, Mr. Pastorius.'
        },
        {
          name:'D:',
          speech:'Good evening, Jake. I think we might have a storm tonight.'
        },
        {
          name:'A:',
          speech:'Oh, really?'
        },
        {
          name:'D:',
          speech:'Yes. The sky’s very dark. And I’ve just heard thunder.'
        },
        {
          name:'A:',
          speech:'Oh, great! I like thunderstorms.'
        },
        {
          name:'D:',
          speech:'I don’t. I’m afraid of the lightning.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'좋은 아침이에요, Libby.'
        },
        {
          name:'B:',
          speech:'안녕하세요, Jake. 날씨가 좋죠, 그렇죠?'
        },
        {
          name:'A:',
          speech:'그래요. 오늘 뭐해요?'
        },
        {
          name:'B:',
          speech:'잘 모르겠어요. 나중에 해변에 갈지도 몰라요.'
        },
        {
          name:'A:',
          speech:'음, 우산을 가지고 가세요. 방금 일기예보를 봤어요. 오늘 오후에 비가 올지도 몰라요'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'A:',
          speech:'안녕하세요, Acuna부인.'
        },
        {
          name:'C:',
          speech:'안녕하세요, Jake. 오늘은 별로 좋지 않지요?'
        },
        {
          name:'A:',
          speech:'좋은 아침이었어요. 곧 비가 그칠지도 몰라요.'
        },
        {
          name:'C:',
          speech:'그러길 바래요.'
        },
        {
          name:'A:',
          speech:'오늘 테니스 치나요?'
        },
        {
          name:'C:',
          speech:'아마 날씨에 따라 다를 거예요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'A:',
          speech:'안녕하세요, 목사님.'
        },
        {
          name:'D:',
          speech:'안녕하세요, Jake. 오늘 밤에 폭풍우가 올 것 같아요.'
        },
        {
          name:'A:',
          speech:'아, 그래요?'
        },
        {
          name:'D:',
          speech:'네. 하늘이 아주 어두워요. 그리고 방금 천둥소리를 들었어요.'
        },
        {
          name:'A:',
          speech:'아, 좋아요! 저는 천둥번개를 좋아합니다.'
        },
        {
          name:'D:',
          speech:'저는 안그래요. 번개가 무서워요.'
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
