<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/two-successful-businessmen-discussing-business_1163-5295.jpg" class="cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 class="upper-header-DBR4">I'll do it
      </h1>
    </v-layout>
  </v-img>

  <hr class="top-line-DBR4">
  <h3 class="lower-header-DBR4">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

    <li style="list-style-type: none;">I'll do it</li><br />

    <table style = "border-collapse: collapse;">
    
      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table>

      <div class="line-DBR4">
      </div>
      <h3 class = "border-DBR4 white--text">Exercise</h3>
        <div style="padding : 16px;">

        <p>
          <u>Fill the blanks.</u><br />
        </p>
        <br />
        <p>
          Requests
        </p>
        <br />
          <li>
            A: <u> &emsp; &emsp; &emsp; </u> you close the door, please? <br />
            B: Yes, I <u> &emsp; &emsp; &emsp; </u>. <br />
          </li>
        <br />
        <p>
          Offers
        </p>
        <br />
          <li>
            A: I'm thirsty. <br />
            B: <u> &emsp; &emsp; &emsp; </u> get you a glass of water. <br />
          </li>
        <br />
        <p>
          Suggestions
        </p>
        <br />
          <li>
            A: There's no food in the fridge. <br />
            B: <u> &emsp; &emsp; &emsp; </u> we go to the restaurant? <br />
          </li>
  
      </div>

      <div class="line-DBR4">
      </div>
      <h3 class = "border-DBR4 white--text">Translation</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr v-for="translation in translations"  :key="translation">
            <td class = "uppertable" >{{translation.name}}</td>
            <td class = "lowertable" >{{translation.speech}}</td>
          </tr>
  
        </table>

        
</div>
        <div class="line-DBR4">
        </div>
        <h3 class = "border-DBR4 white--text">Self Study</h3>
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
                      조동사 will : 1. 고집, 주장을 나타낼 때 (어떻게든 ~하려고 하다)<br />
                              2. 현재의 습관, 습성, 경향을 나타낼 때 (~하곤한다, ~하기 마련이다)<br />
                              3. 현재의 추측을 나타낼 때 (~일 것이다)<br />
                              4. 부탁할 때 (~해주시겠습니까?)<br />
                              <br />
                              Ex) Will you open the window, please? : 창문 좀 열어주시겠습니까?<br />
                                   I'll get you a glass of iced water, too : 얼음 물 한잔도 가져 오겠습니다<br />
                                   I'll get it right away : 지금 바로 가져오겠습니다<br />
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
          name:'Mr. Burnette:',
          speech:'Come in!'
        },
        {
          name:'Withers:',
          speech:'Sir?'
        },
        {
          name:'Mr. B:',
          speech:'Who are you?'
        },
        {
          name:'Withers:',
          speech:'My name’s Withers, sir. I’m your new personal assistant.'
        },
        {
          name:'Mr. B:',
          speech:'Where’s Mrs. Sherman? I want my coffee!'
        },
        {
          name:'Withers:',
          speech:'I’ll get it, sir.'
        },
        {
          name:'Mr. B:',
          speech:'Thank you, Smithers.'
        },
        {
          name:'Withers:',
          speech:'Uh ... it’s “Withers”, sir.'
        },
        {
          name:'Mr. B:',
          speech:'It’s hot in here. Will you open the window, please?'
        },
        {
          name:'Withers:',
          speech:'Yes, sir. I’ll get you a glass of iced water, too.'
        },
        {
          name:'Mr. B:',
          speech:'Good. Please be quick.'
        },
        {
          name:' ',
          speech:'Will you bring me the “suggestions” box, Withers?'
        },
        {
          name:'Withers:',
          speech:'Of course I will, sir. Uh ... where is it?'
        },
        {
          name:'Mr. B:',
          speech:'In the cafeteria. People can put suggestions about the company in it.'
        },
        {
          name:'Withers:',
          speech:'I’ll get it right away.'
        },
        {
          name:'Mr. B:',
          speech:'All right, Blithers. Let’s see it!'
        },
        {
          name:'Withers:',
          speech:'There are a lot of suggestions, sir.'
        },
        {
          name:'Mr. B:',
          speech:'Well, let’s hear them!'
        },
        {
          name:'Withers:',
          speech:'Yes, sir. This is the first one. “Why doesn’t Burnette speak politely to people?” Next, “Why don’t the bosses remember our names?” And another, “Why don’t we begin work at 11 AM? Old Burnette does.” And another...'
        },
        {
          name:'Mr. B:',
          speech:'“Old Burnette,” eh? Who wrote the suggestions? Did they sign them?'
        },
        {
          name:'Withers:',
          speech:'Uh, no, sir.'
        },
        {
          name:'Mr. B:',
          speech:'Find their names, Withers.'
        },
        {
          name:'Withers:',
          speech:'I will, sir.'
        },
        {
          name:'Mr. B:',
          speech:'And don’t tell anybody about the suggestions.'
        },
        {
          name:'Withers:',
          speech:'I won’t, sir.'
        },
        ],

        translations:[
        {
          name:'Mr. Burnette:',
          speech:'들어오세요!'
        },
        {
          name:'Withers:',
          speech:'선생님?'
        },
        {
          name:'Mr. B:',
          speech:'누구세요?'
        },
        {
          name:'Withers:',
          speech:'제 이름은 Withers입니다. 저는 당신의 새로운 개인 비서입니다.'
        },
        {
          name:'Mr. B:',
          speech:'부인은 어디 있어요. Mrs. Sherman이라고요? 커피 주세요!'
        },
        {
          name:'Withers:',
          speech:'알겠습니다, 손님.'
        },
        {
          name:'Mr. B:',
          speech:'스미더스 씨, 감사합니다.'
        },
        {
          name:'Withers:',
          speech:'어... "Withers"입니다.'
        },
        {
          name:'Mr. B:',
          speech:'이 안이 더워요. 창문 좀 열어 주시겠어요?'
        },
        {
          name:'Withers:',
          speech:'네, 알겠습니다. 얼음물도 한 잔 가져다드릴게요.'
        },
        {
          name:'Mr. B:',
          speech:'좋습니다. 빨리 좀 해 주세요.'
        },
        {
          name:' ',
          speech:'Withers, 저에게 "제안" 상자를 가져다 주시겠어요?'
        },
        {
          name:'Withers:',
          speech:'물론 그렇게 하겠습니다, 선생님. 어... 어디있죠?'
        },
        {
          name:'Mr. B:',
          speech:'카페테리아에서요. 사람들은 그 회사에 대해 제안할 수 있습니다.'
        },
        {
          name:'Withers:',
          speech:'당장 갖다 드리겠습니다.'
        },
        {
          name:'Mr. B:',
          speech:'좋아요, Blithers. 어디 봐요!'
        },
        {
          name:'Withers:',
          speech:'여러 가지 제안이 있습니다.'
        },
        {
          name:'Mr. B:',
          speech:'음, 들어봐요!'
        },
        {
          name:'Withers:',
          speech:'네, 알겠습니다. 이게 첫 번째예요. "Burnette은 왜 사람들에게 공손하게 말을 하지 않는 거죠?" 다음으로, "왜 사장님들은 우리 이름을 기억 못 하시나요?" 그리고 또 다른 것은, "아침 11시에 일을 시작하는 게 어때요? Old Burnette은 그래요." 그리고 또 다른 것은요...'
        },
        {
          name:'Mr. B:',
          speech:'"Old Burnette"이라고요? 누가 제안서를 썼나요? 그들이 서명했나요?'
        },
        {
          name:'Withers:',
          speech:'어, 아닙니다.'
        },
        {
          name:'Mr. B:',
          speech:'Withers 씨, 그들의 이름을 찾아보세요.'
        },
        {
          name:'Withers:',
          speech:'그러겠습니다.'
        },
        {
          name:'Mr. B:',
          speech:'그리고 그 제안들에 대해 아무에게도 말하지 마세요.'
        },
        {
          name:'Withers:',
          speech:'안 할게요.'
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

</style>
