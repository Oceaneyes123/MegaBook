<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/upset-woman-standing-near-rack-clothes-chatting-smart-phone-with-her-friend-complaining-that-she-has-nothing-wear-displeased-female-knowing-what-put-birthday-party_273609-185.jpg" class="cover-photo">

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
        padding-bottom: 10px;">I hate my job
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">I hate my job</li><br />
      <br />
      <p>
        Sandra works as a hotel receptionist. She’s unhappy with her job. She doesn’t like her boss and her coworkers. She works long hours, but doesn’t earn very much. She needs a change, but doesn’t know what to do. She’s now talking to her friend, Amanda, about the situation.<br />
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
            Do you like your job?
          </li>
          <li>
            What are the good things about your job? What are the bad things?
          </li>
          <li>
            Do you like your boss?
          </li>
          <li>
            What are your coworkers like?
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
          Sandra는 호텔 접수원으로 일합니다. 그녀는 자기 일에 불만이 있어요. 그녀는 그녀의 상사와 동료들을 좋아하지 않아요. 그녀는 장시간 일하지만, 수입이 별로 없어요. 그녀는 변화가 필요하지만 어떻게 해야 할지 모르겠어요. 그녀는 지금 그녀의 친구 Amanda와 그 상황에 대해 이야기하고 있습니다.<br />
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
                      의문사 + to부정사 : how, where, what, when등의 의문사에 to부정사가 붙은 형태로 주로 know, tell, ask 등의 목적어로 쓰입니다. <br />                 
                      how + to부정사 : 어떻게 ~할지 / where + to부정사 : 어디에 ~할지 / what + to부정사 : 무엇을 ~할지 / when + to부정사 : 언제 ~할지<br />                  
                      <br />
                        Ex) She doesn't know what to do : 그녀는 무엇을 할지를 모른다.<br />
                          Tell me when to open the door : 문을 언제 열어야 할지를 나에게 말해주시오.<br />
                    </li>
                    <li>
                      관계대명사 what : the thing과 관계대명사 which(that)을 대신하는 것으로 ~한 것이라고 해석합니다.<br />
                    </li>
                    <li>
                      talk to + (주로)사람 : ~에게 이야기하다, talk about + 대화 주제 : ~에 대해 이야기하다
                    </li>
                    <li>
                      work with : ~와 함께 일하다
                    </li>
                    <li>
                      salary is very low : 월급이 너무 적다
                    </li>
                    <li>
                      ask A for B : A에게 B를 요구하다
                    </li>
                    <li>
                      shout at : ~에게 소리지르다
                    </li>
                    <li>
                      You'll be much happier : 너는 훨씬 행복해질거야
                    </li>
                    <li>
                      I'm sure you can ... : 너가 ~할 수 있다고 확신한다
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
          speech:'I hate my job. It’s so boring.'
        },
        {
          name:'B:',
          speech:'I know what you mean. You’d like a more interesting job, right?'
        },
        {
          name:'A:',
          speech:'My coworkers at the hotel aren’t very nice.'
        },
        {
          name:'B:',
          speech:'I’m sorry to hear that. You need to work with nicer people.'
        },
        {
          name:'A:',
          speech:'I’m so tired. I have to work long hours.'
        },
        {
          name:'B:',
          speech:'That’s too bad. Ask your boss if you can work shorter hours.'
        },
        {
          name:'A:',
          speech:'And my salary is very low, only a thousand dollars a month.'
        },
        {
          name:'B:',
          speech:'Is that all? You need a job that pays a higher salary.'
        },
        {
          name:'A:',
          speech:'I asked my boss for a raise, but he said no. He’s very stingy.'
        },
        {
          name:'B:',
          speech:'He should be more generous.'
        },
        {
          name:'A:',
          speech:'He’s always shouting at me. He’s so rude.'
        },
        {
          name:'B:',
          speech:'That’s terrible! You need to work for someone who is more polite.'
        },
        {
          name:'A:',
          speech:'I’m so depressed. I don’t know what to do.'
        },
        {
          name:'B:',
          speech:'Get another job. You’ll be much happier.'
        },
        {
          name:'A:',
          speech:'You’re right. But it’s hard to find a good job.'
        },
        {
          name:'B:',
          speech:'It’s not impossible. I’m sure you can find a better job than the one you have now.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'난 내 일이 싫어. 너무 지루해.'
        },
        {
          name:'B:',
          speech:'무슨 말인지 알아. 좀 더 흥미로운 직업을 원하겠지?'
        },
        {
          name:'A:',
          speech:'호텔 동료들이 별로 안 좋아.'
        },
        {
          name:'B:',
          speech:'안됐구나. 너는 더 좋은 사람들과 함께 일해야 해.'
        },
        {
          name:'A:',
          speech:'너무 피곤해. 나는 장시간 일해야 해.'
        },
        {
          name:'B:',
          speech:'안됐네. 상사에게 더 짧은 시간을 일할 수 있는지 물어봐라.'
        },
        {
          name:'A:',
          speech:'그리고 내 월급은 한 달에 천 달러밖에 안 돼.'
        },
        {
          name:'B:',
          speech:'그게 다야? 봉급이 더 높은 직장이 필요해.'
        },
        {
          name:'A:',
          speech:'사장님께 월급을 올려 달라고 했는데 안 된다고 했어. 그는 매우 인색해.'
        },
        {
          name:'B:',
          speech:'그는 좀 더 관대해야 해.'
        },
        {
          name:'A:',
          speech:'그는 항상 나한테 소리쳐. 그는 너무 무례해.'
        },
        {
          name:'B:',
          speech:'끔찍해! 너는 좀 더 예의 바른 사람을 위해 일해야 해.'
        },
        {
          name:'A:',
          speech:'너무 우울해. 어떻게 해야 할지 모르겠어.'
        },
        {
          name:'B:',
          speech:'다른 직장을 구해. 넌 훨씬 더 행복해질 거야.'
        },
        {
          name:'A:',
          speech:'네 말이 맞아. 하지만 좋은 직장을 구하기는 어려워.'
        },
        {
          name:'B:',
          speech:'불가능하지는 않아. 나는 네가 지금 가지고 있는 것보다 더 좋은 직업을 찾을 수 있을 거라고 확신해.'
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
