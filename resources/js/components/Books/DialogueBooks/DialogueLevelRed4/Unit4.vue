<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/businessman-talking-phone_58466-11186.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Wrong number
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Wrong number</li><br />

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
            Who did Ms O’Conner want to call?<br />
          </li>
          <li>
            Who did she talk to?<br />
          </li>
          <li>
            What number did she want to call?<br />
          </li>
          <li>
            Why did she call?<br />
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
                      I wanted to see you : 나는 당신을 보기를 원했습니다 <br />
                    </li>
                    <li>
                      I had to see my doctor : 나는 의사를 만나야 했습니다 <br />
                    </li>
                    <li>
                      to have problems with ~ : ~에 문제가 있다 <br />
                    </li>
                    <li>
                      I wanted to ask you about your account : 나는 당신의 계좌에 대해 묻고 싶었습니다 <br />
                    </li>
                    <li>
                      You have the wrong number : 전화 잘못 하셨습니다 <br />
                    </li>
                    <li>
                      to write a check for $... :  ...달러 라고 쓰다. <br />
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
          speech:'Hello.'
        },
        {
          name:'B:',
          speech:'Good morning. This is the First State Bank. My name’s Bridget O’Connor. I’m the manager.'
        },
        {
          name:'A:',
          speech:'Oh, yes?'
        },
        {
          name:'B:',
          speech:'Did you get my letter?'
        },
        {
          name:'A:',
          speech:'What letter was that?'
        },
        {
          name:'B:',
          speech:'Well, I wanted to see you. I called yesterday, but I couldn’t get an answer.'
        },
        {
          name:'A:',
          speech:'Was that in the morning?'
        },
        {
          name:'B:',
          speech:'That’s right.'
        },
        {
          name:'A:',
          speech:'I’m sorry, I wasn’t here. I had to see my doctor. I had problems with my leg.'
        },
        {
          name:'B:',
          speech:'I wanted to ask you about your account.'
        },
        {
          name:'A:',
          speech:'My account?'
        },
        {
          name:'B:',
          speech:'Yes. You wrote a check for $1,000 last week.'
        },
        {
          name:'A:',
          speech:'$1,000??'
        },
        {
          name:'B:',
          speech:'Yes, and there’s only $152.95 in your account.'
        },
        {
          name:'A:',
          speech:'But I don’t have an account with First State.'
        },
        {
          name:'B:',
          speech:'Now, look here Mr. Trump...'
        },
        {
          name:'A:',
          speech:'Mr. Trump? Who’s Mr. Trump? I’m not Mr. Trump.'
        },
        {
          name:'B:',
          speech:'I’m sorry. Is this 848-3592?'
        },
        {
          name:'A:',
          speech:'Say that again.'
        },
        {
          name:'B:',
          speech:'848-3592.'
        },
        {
          name:'A:',
          speech:'Ah! This is 848-3952. My name’s Sikorsky. You have the wrong number.'
        },
        {
          name:'B:',
          speech:'Oh! Sorry.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'안녕하세요.'
        },
        {
          name:'B:',
          speech:'좋은 아침이에요. 이것은 First State 은행입니다. 제 이름은 Bridget O’Connor입니다 저는  매니저입니다.'
        },
        {
          name:'A:',
          speech:'아, 그래요?'
        },
        {
          name:'B:',
          speech:'제 편지 받았어요?'
        },
        {
          name:'A:',
          speech:'무슨 편지였어요?'
        },
        {
          name:'B:',
          speech:'음, 보고 싶었어요. 어제 전화했는데 받지 않았어요.'
        },
        {
          name:'A:',
          speech:'그게 아침이었어요?'
        },
        {
          name:'B:',
          speech:'맞아요.'
        },
        {
          name:'A:',
          speech:'죄송해요, 전 여기 없었어요. 의사에게 진찰을 받아야 했어요. 다리에 문제가 생겼어요.'
        },
        {
          name:'B:',
          speech:'계좌에 대해 물어보고 싶었어요.'
        },
        {
          name:'A:',
          speech:'제 계좌요?'
        },
        {
          name:'B:',
          speech:'네. 지난주에 1,000달러짜리 수표를 썼잖아요.'
        },
        {
          name:'A:',
          speech:'1,000달러요?'
        },
        {
          name:'B:',
          speech:'네, 그리고 당신 계좌에는 152달러 95센트밖에 없어요.'
        },
        {
          name:'A:',
          speech:'하지만 퍼스트 스테이트와 거래하는 계좌가 없어요.'
        },
        {
          name:'B:',
          speech:'자, 여기 보세요, Trump씨...'
        },
        {
          name:'A:',
          speech:'Trump씨요? Trump씨가 누구죠? 저는 Trump 대통령이 아닙니다.'
        },
        {
          name:'B:',
          speech:'죄송합니다. 여기가 848-3592입니까?'
        },
        {
          name:'A:',
          speech:'다시 한 번 말씀해 보세요.'
        },
        {
          name:'B:',
          speech:'848-3592입니다.'
        },
        {
          name:'A:',
          speech:'아! 여기는 848-3952입니다. 제 이름은 Sikorsky입니다. 전화를 잘못 거셨습니다.'
        },
        {
          name:'B:',
          speech:'아! 미안해요.'
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
