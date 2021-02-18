<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/businesspeople-floating-with-suitcase_23-2148186803.jpg" class="cover-photo">

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
        padding-bottom: 10px;">You’re late!
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">You’re late!</li><br />

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
          <u>Complete the conversations. Use the present perfect and simple past of the verbs given</u><br />
              Example:<br />
                  A: Have you ever sung in a karaoke bar?  ( sing )<br />
                  B: Yes, I have. I sang in one on my birthday.<br />    
        </p>

        <ol style="margin: 12px;">
          <li>
           <br />
              A: <u> &emsp; &emsp; &emsp; </u> you ever <u> &emsp; &emsp; &emsp; </u> something valuable? ( lose ) <br />
              B: No, I <u> &emsp; &emsp; &emsp; </u>. But my brother <u> &emsp; &emsp; &emsp; </u> his camera on a trip once. <br />           
          </li>
          <li>
            <br />
              A: <u> &emsp; &emsp; &emsp; </u> you ever <u> &emsp; &emsp; &emsp; </u> a traffic ticket? ( get ) <br />
              B: Yes, I <u> &emsp; &emsp; &emsp; </u>. Once I <u> &emsp; &emsp; &emsp; </u> a ticket and had to pay $50. <br />           
          </li>
          <li>
            <br />
              A: <u> &emsp; &emsp; &emsp; </u> you ever <u> &emsp; &emsp; &emsp; </u> late for an important appointment? ( be ) <br />
              B: No, I <u> &emsp; &emsp; &emsp; </u>. But my friend <u> &emsp; &emsp; &emsp; </u> 30 minutes late for her wedding! <br />           
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
                      과거시제와 함께 쓰이는 표현들 : 과거의 특정 시점을 나타내는 부사구와 함께 쓰입니다. in+연도, last night(week), yesterday, When~?<br />
                    </li>
                    <li>
                      현재완료와 함께 쓰이는 표현들 : 현재완료의 용법에 따라 현재완료와 주로 쓰이는 부사구가 있습니다.<br />                 
                          경험 : ever, never, once, twice, ~times, before<br />
                          계속 : How long~?, for+기간, since+기점<br />
                          완료 : already(벌써,이미), yet(아직 ~하지 않은), just(지금,막)<br />
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
          speech:'I’m sorry I’m late. Have you been here long?'
        },
        {
          name:'B:',
          speech:'No, only for a few minutes.'
        },
        {
          name:'A:',
          speech:'Have you chosen a restaurant yet?'
        },
        {
          name:'B:',
          speech:'I can’t decide. Have you ever eaten Moroccan food?'
        },
        {
          name:'A:',
          speech:'No, I haven’t. Is it good?'
        },
        {
          name:'B:',
          speech:'It’s delicious. I’ve had it several times.'
        },
        {
          name:'A:',
          speech:'Or how about Thai food? Have you ever had green curry?'
        },
        {
          name:'B:',
          speech:'Actually, I have. I lived in Thailand as a teenager. I ate it a lot there.'
        },
        {
          name:'A:',
          speech:'I didn’t know that. How long did you live there?'
        },
        {
          name:'B:',
          speech:'I lived there four years.'
        },
        {
          name:'A:',
          speech:'So what about dinner? I’m hungry!'
        },
        {
          name:'B:',
          speech:'Have you tried Sakura? They have excellent sushi.'
        },
        {
          name:'A:',
          speech:'Actually, I had Japanese food for lunch.'
        },
        {
          name:'B:',
          speech:'Well, should we have Italian food? Café Roma is a great place, and it isn’t far.'
        },
        {
          name:'A:',
          speech:'That’s fine with me. I love Italian food.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'늦어서 미안해. 여기 오래 있었니?'
        },
        {
          name:'B:',
          speech:'아니, 몇 분만.'
        },
        {
          name:'A:',
          speech:'식당 정했어?'
        },
        {
          name:'B:',
          speech:'결정할 수가 없어. 모로코 음식을 먹어본 적이 있니?'
        },
        {
          name:'A:',
          speech:'아니, 못 봤어. 좋아?'
        },
        {
          name:'B:',
          speech:'맛있어. 여러 번 먹어본 적이 있어.'
        },
        {
          name:'A:',
          speech:'아니면 태국 음식은 어때? 너는 녹색 카레를 먹어본 적이 있니?'
        },
        {
          name:'B:',
          speech:'사실, 그랬어. 나는 10대 때 태국에서 살았어. 거기서 많이 먹었어.'
        },
        {
          name:'A:',
          speech:'그건 몰랐어. 거기서 얼마나 살았니?'
        },
        {
          name:'B:',
          speech:'나는 그곳에서 4년을 살았어.'
        },
        {
          name:'A:',
          speech:'그럼 저녁은 어때? 배고파!'
        },
        {
          name:'B:',
          speech:'사쿠라 먹어봤어? 그들은 훌륭한 초밥을 가지고 있어.'
        },
        {
          name:'A:',
          speech:'사실, 점심으로 일본 음식을 먹었어.'
        },
        {
          name:'B:',
          speech:'그럼 이탈리아 음식 먹을까? 카페로마는 멋진 곳이고, 멀지 않아.'
        },
        {
          name:'A:',
          speech:'난 괜찮아. 나는 이탈리아 음식을 좋아해.'
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
