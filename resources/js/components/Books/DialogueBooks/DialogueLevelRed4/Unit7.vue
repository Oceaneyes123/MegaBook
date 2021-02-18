<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/adorable-brunette-young-woman-with-beautiful-hair-keeping-hands-together-praying_176532-10478.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Asking for favor
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Asking for favor</li><br />

      <br />
      <p>
        Would you do me a favor?<br />
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
          <u>Have similar conversations</u><br />
        </p>
        <br />
        <li>
          A: Would (Could) you do me a favor, <u> &emsp; &emsp; &emsp; </u>? <br />
          B: What is it? <br />
          A: Would (Could) you, <u> &emsp; &emsp; &emsp; </u>? <br />
          B: Yeah, sure. I’ll be happy to. OR No, I can’t. I don’t have time. <br />
        </li>

        <p>
          Example:<br />
          Would you...<br />
          <br />
          <u> &emsp; &emsp; &emsp; </u> return this book to the library?<br />
          <u> &emsp; &emsp; &emsp; </u> make me a cup of coffee?<br />
          <u> &emsp; &emsp; &emsp; </u> wash the dishes?<br />
          <u> &emsp; &emsp; &emsp; </u> water the plants?<br />
          <u> &emsp; &emsp; &emsp; </u> go to the market for me?<br />
          <u> &emsp; &emsp; &emsp; </u> carry this suitcase for me?<br />
          <u> &emsp; &emsp; &emsp; </u> loan me five dollars?<br />
        </p>
        <br />

        <p>
          Say ‘yes’: Say ‘no’:<br />
        </p>
        <br />
        <p>
          Yeah. /Yes. No.<br />
          Sure. I’m sorry.<br />
          OK. I can’t.<br />
          Of course. Not right now.<br />
          No problem. I’m busy.<br />
          I’ll be happy to. I don’t have time.<br />
          It’s a pleasure. I’m too tired.<br />
        </p>
        <br />
        
        <p>
          Free response:<br />
          <br />
          When was the last time you did someone a favor? What was it?<br />
          Are people often asking you a favor? What do they mostly ask for?<br />
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

        <p>
          제 부탁 하나 들어주시겠어요?<br />
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
                      Would you do me a favor? (부탁 좀 드려도 될까요?) = Could you do me a favor? = Will you do me a favor?<br />
                    </li>
                    <li>
                      Would you mail these letters for me? : 날 위해(나 대신) 이 편지 좀 부쳐주실래요? 나 대신 보내달라고 표현할 때에는 for me, 나에게 보내달라고 할 때에는 to me를 씁니다.<br />
                    </li>
                    <li>
                      to get off work (퇴근하다) = to be gone for the day<br >
                    </li>
                    <li>
                      won't be able to (~할 수 없을 것이다) : won't는 will not의 줄임말이고 be able to는 can과 바꿔쓸 수 있는데 won't 뒤에 can이 오지 않은 것은 조동사를 반복해서 사용하지 않기 때문입니다.<br />          
                    </li>
                    <li>
                      stop by : ~에 들르다<br />
                    </li>
                    <li>
                      pick up (some groceries) : ~을 사다, ~을 가지러 가다<br />
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
          speech:'Would you do me a favor, Anne?'
        },
        {
          name:'B:',
          speech:'What is it?'
        },
        {
          name:'A:',
          speech:'Would you mail these letters for me?'
        },
        {
          name:'B:',
          speech:'No, I can’t. I don’t have time.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'Hello.'
        },
        {
          name:'D:',
          speech:'Hi, Mandy. It’s Jill. I’m still at work.'
        },
        {
          name:'C:',
          speech:'Work? I thought you got off work at 5:00.'
        },
        {
          name:'D:',
          speech:'I had to meet the boss. Listen. Could you do me a favor?'
        },
        {
          name:'C:',
          speech:'Sure. What do you need?'
        },
        {
          name:'D:',
          speech:'I won’t be able to stop by the store today. Could you pick up some groceries?'
        },
        {
          name:'C:',
          speech:'OK. No problem.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'Mandy, 제 부탁 좀 들어주시겠어요?'
        },
        {
          name:'B:',
          speech:'뭐예요?'
        },
        {
          name:'A:',
          speech:'이 편지 좀 부쳐 주시겠어요?'
        },
        {
          name:'B:',
          speech:'아니요, 전 못해요. 시간이 없어요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'안녕하세요.'
        },
        {
          name:'D:',
          speech:'안녕하세요, Mandy. Jill이에요. 저는 아직 직장에 있어요.'
        },
        {
          name:'C:',
          speech:'일해요? 5시에 퇴근한 줄 알았어요.'
        },
        {
          name:'D:',
          speech:'사장님을 만나야 했어요. 들어보세요 제 부탁 하나 들어주시겠어요?'
        },
        {
          name:'C:',
          speech:'물론이죠. 뭐가 필요하신가요?'
        },
        {
          name:'D:',
          speech:'오늘은 가게에 들를 수 없을 것 같아요. 식료품 좀 사다 줄래요?'
        },
        {
          name:'C:',
          speech:'알았어요. 문제없어요.'
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
