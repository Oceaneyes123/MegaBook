<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/elderly-doctor-listening-young-patient_23-2147896642.jpg" class="cover-photo">

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
        padding-bottom: 10px;">At a doctor
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">At a doctor</li><br />

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
          <u>Look at the pictures and match the dialogs</u><br />
        </p>
        <br />
        <table style = "border-collapse: collapse;">

          <tr v-for="item in items" :key="item">
            <td class = "uppertable" >{{item.a}}</td>
            <td class = "lowertable" >{{item.b}}</td>
          </tr>
  
        </table>
        <br />
        <v-container grid-list-md text-xs-center>
          <v-layout wrap align-content-center>
          
            <v-flex xs12 md6 >
              <v-card hover>
          
                <v-img src="images/orlando.png" />
          
              </v-card>
            </v-flex>
          
          </v-layout>
        
        </v-container>

        <br />
        <p>
          Free response:<br />
          <br />
          Talk about health<br />
          <br />
          Example:<br />
              Do you exercise regularly? How?<br />
              How do you relax?<br />
              How much sleep do you get? Is that enough?<br />
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
                      should : 조동사로 ~해야 한다, ~하는 것이 좋겠다는 뜻으로 의무나 충고를 나타냅니다. 부정은 should 뒤에 not을 붙입니다. <br />
                    </li>
                    <li>
                      make + 목적어 + 목적격보어(형용사) : 목적격 보어로 형용사가 올 경우, 형용사는 목적어의 상태를 설명합니다. 목적어를 목적격보어하게 하다<br />
                    </li>
                    <li>
                      to부정사 *형용사적 용법 : 명사뒤에서 명사를 수식할 때 to부정사는 형용사처럼 쓰입니다. <br />
                          (the only way to lose weight: 살을 빼는 유일한 방법)<br />
                          <br />
                              *명사적 용법 : 문장에서 주어를 보충 설명하는 보어의 역할을 합니다.<br />
                              (the only way to lose weight is to exercise more and eat less: 살을 빼는 유일한 길은 더 열심히 운동하고 더 적게 먹는 것이다)<br />
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
          speech:'How are you, Albert?'
        },
        {
          name:'B:',
          speech:'Not very well, Doctor. I feel tired all the time.'
        },
        {
          name:'A:',
          speech:'You should get more sleep.'
        },
        {
          name:'B:',
          speech:'I get plenty of sleep. But I don’t seem to have any energy.'
        },
        {
          name:'A:',
          speech:'That’s because you’re overweight. You shouldn’t eat so much.'
        },
        {
          name:'B:',
          speech:'You mean I should go on a diet?'
        },
        {
          name:'A:',
          speech:'That’s right. And you should exercise more. Take up a sport.'
        },
        {
          name:'B:',
          speech:'Well, I was going to play on the basketball team this year. But the coach said I was too slow.'
        },
        {
          name:'A:',
          speech:'You should run more to get in shape.'
        },
        {
          name:'B:',
          speech:'I did a lot of running last year. But it made me very hungry, so I stopped.'
        },
        {
          name:'A:',
          speech:'You shouldn’t give up, Albert. Just remember, the only way to lose weight is to exercise more and eat less.'
        },
        {
          name:'B:',
          speech:'OK, Doctor. I’ll do my best.'
        },
        ],

        items:[
        {
          a:'I’m out of shape.',
          b:'You shouldn’t play with matches.'
        },
        {
          a:'I have a headache.',
          b:'You should exercise more.'
        },
        {
          a:'I can’t sleep.',
          b:'You should get some rest.'
        },
        {
          a:'I burned my finger.',
          b:'You should take an aspirin.'
        },
        {
          a:'I’m tired.',
          b:'You shouldn’t lift heavy objects.'
        },
        {
          a:'My back is sore.',
          b:'You shouldn’t drink coffee.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'안녕하세요, Albert?'
        },
        {
          name:'B:',
          speech:'잘 안 돼요, 의사선생님. 저는 항상 피곤해요.'
        },
        {
          name:'A:',
          speech:'잠을 더 자야 해요'
        },
        {
          name:'B:',
          speech:'잠을 충분히 자요. 그런데 기운이 하나도 없는 것 같아요.'
        },
        {
          name:'A:',
          speech:'그건 당신이 과체중이기 때문이에요. 그렇게 많이 먹으면 안 돼요.'
        },
        {
          name:'B:',
          speech:'다이어트를 해야 한다는 말인가요?'
        },
        {
          name:'A:',
          speech:'맞아요. 그리고 운동을 더 많이 해야 합니다. 운동을 하세요.'
        },
        {
          name:'B:',
          speech:'음, 저는 올해 농구팀에서 뛸 예정이었어요. 하지만 코치는 내가 너무 심하다고 말했어요. 천천히요.'
        },
        {
          name:'A:',
          speech:'몸매를 가꾸려면 더 많이 뛰어야 해요.'
        },
        {
          name:'B:',
          speech:'작년에 달리기를 많이 했어요. 하지만 그것은 저를 매우 배고프게 만들었고, 그래서 저는 그만뒀습니다.'
        },
        {
          name:'A:',
          speech:'Albert, 포기하면 안 돼요. 살을 빼는 유일한 방법은 운동을 하는 것입니다. 더 많이 먹고 적게 먹어요.'
        },
        {
          name:'B:',
          speech:'알았어요, 의사선생님. 최선을 다하겠습니다.'
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
