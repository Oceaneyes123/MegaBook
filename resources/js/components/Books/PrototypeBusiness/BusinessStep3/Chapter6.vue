<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGv4WssmY/7/screen_2x/canva-flat-screen-television-MADGv4WssmY.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Talking about your interests
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
            Why doesn’t the man watch football on TV?
          </li>
          <li>
            Why does he talk about polo?
          </li>
          <li>
            What’s he interested in, apart from golf?
          </li>
        </ol>

        <p>
           Free response:<br />
           What are the most popular sports and leisure activities in your country?<br />
           What do you think the most popular sports and leisure activities in the world are?
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
                  Useful language:<br />
                  I enjoy playing golf. / I can’t stand football! / I like watching ice skating<br />
                  I’m hopeless at tennis! / I’d love to have a go at surfing / I’m (not) interested in that
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
          name:'Woman:',
          speech:'So, are you watching the cup final this weekend?'
        },
        {
          name:'Man:',
          speech:'Um… no, I don’t think so.'
        },
        {
          name:'Woman:',
          speech:'Don’t you like football?'
        },
        {
          name:'Man:',
          speech:'No. I can’t stand it. Sorry to sound so miserable!'
        },
        {
          name:'Woman:',
          speech:'Mmm, I hate it too, but I watch the World Cup Final.'
        },
        {
          name:'Man:',
          speech:'I can’t play, that’s my problem. I’m hopeless at it! If I’m not very good at a sport, I don’t like watching it.'
        },
        {
          name:'Woman:',
          speech:'So what do you like, then?'
        },
        {
          name:'Man:',
          speech:'I play golf.'
        },
        {
          name:'Woman:',
          speech:'Oh right… My husband plays. I’m not interested in it, though. It’s…not my cup of tea. He plays golf, I go horse riding.'
        },
        {
          name:'Man:',
          speech:'Oh, right. Well you could play polo-both of you. That’s half horse riding, half golf!... I’d love to have a go at riding, actually. I bet it’s good fun.'
        },
        {
          name:'Woman:',
          speech:'Oh, it’s great fun.'
        },
        {
          name:'Man:',
          speech:'So, do you have your own horse?'
        },
        {
          name:'Woman:',
          speech:'No. I’d love to have one, but, um…it’s expensive.'
        },
        {
          name:'Man:',
          speech:'Yeah, I’m quite interested in tropical fish. I’d like to have an aquarium, but…it’s a problem if you travel a lot…'
        },
        {
          name:'Woman:',
          speech:'Tropical fish?'
        },
        {
          name:'Man:',
          speech:'Yeah. I’d like to have some piranhas.'
        },
        {
          name:'Woman:',
          speech:'Piranhas?'
        },
        {
          name:'Man:',
          speech:'Well, they say a hundred piranhas can eat a horse in less than five minutes!'
        },
        {
          name:'Woman:',
          speech:'Oh!'
        },
        {
          name:'Man:',
          speech:'I’m not sure if that includes the rider or not…'
        },
        ],

        translations:[
        {
          name:'W:',
          speech:'그래, 이번 주말에 컵 결승전을 볼 거야?'
        },
        {
          name:'M:',
          speech:'음… 아니, 별로.'
        },
        {
          name:'W:',
          speech:'넌 축구를 좋아하지 않니?'
        },
        {
          name:'M:',
          speech:'응. 견딜 수 없어 . 너무 비참하게 말해서 미안해!'
        },
        {
          name:'W:',
          speech:'음, 나도 싫어. 하지만 난 월드컵 결승전은 봐.'
        },
        {
          name:'M:',
          speech:'난 경기를 할 수 없어. 그게 내 문제야. 난 그걸 할 가망이 없어! 만약 내가 스포츠를 잘하지 못한다면, 나는 그것을 보는 것을 좋아하지 않아.'
        },
        {
          name:'W:',
          speech:'그럼, 넌 뭐가 좋아?'
        },
        {
          name:'M:',
          speech:'난 골프를 쳐.'
        },
        {
          name:'W:',
          speech:'오, 맞다… 남편이 골프를 쳐. 그래도 난 관심 없어. 그건 내 취향이 아니야. 그는 골프를 치고 나는 말을 타러 가.'
        },
        {
          name:'M:',
          speech:'오, 맞아. 너희 둘 다 폴로를  할 수 있잖아. 반은 승마, 반은 골프! 사실 나도 한번 타보고 싶어. 정말 재미있을 거야.'
        },
        {
          name:'W:',
          speech:'오, 정말 재미있어.'
        },
        {
          name:'M:',
          speech:'그래, 네 말은 있어?'
        },
        {
          name:'W:',
          speech:'아니. 나도 하나 갖고 싶지만, 음... 비싸.'
        },
        {
          name:'M:',
          speech:'그래, 난 열대어에 꽤 관심이 있어. 나는 수족관을 갖고 싶은데, 여행을 많이 하면 문제가 되잖아.'
        },
        {
          name:'W:',
          speech:'열대어?'
        },
        {
          name:'M:',
          speech:'그래. 피라냐를 가지고 싶어.'
        },
        {
          name:'W:',
          speech:'피라냐?'
        },
        {
          name:'M:',
          speech:'글쎄, 그들은 피라냐 백 마리가 5분도 안 돼서 말을 먹을 수 있다고 해!'
        },
        {
          name:'W:',
          speech:'오!'
        },
        {
          name:'M:',
          speech:'기수를 포함한 건지 아닌지는 잘 모르겠어.'
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
