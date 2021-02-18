<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/businessman-his-office-with-magnifying-glass_1368-4641.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Investigation
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Investigation</li><br />
    <br />
      <p>
        Last night at 9:18 PM, Mr. Scott Shaw, a high school principal, was walking from his office to his car when he was attacked from behind. The attacker hit the principal on the head. The police think the attacker was a student. They are going to question every student in the school — both male and female. A police officer questioned the victim at the hospital last night:<br />
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
          <u>Answer the questions.</u><br />
        </p>

        <ol style="margin: 12px;">
          <li>
            When was Mr. Shaw attacked?<br />
          </li>
          <li>
            What was he doing when the attack happened?<br />
          </li>
          <li>
            How did he break his leg?<br />
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
          어젯밤 9시 18분, 고등학교 교장인 Scott Shaw 씨가 사무실에서 차로 걸어가다가 뒤에서 공격을 받았습니다. 그 공격자는 교장 선생님의 머리를 때렸습니다. 경찰은 그 공격자가 학생이었다고 생각합니다. 그들은 학교의 모든 남학생과 여학생 모두를 심문할 것입니다. 한 경찰관이 어젯밤 병원에서 피해자를 심문했습니다.<br />
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
                      6 feet 2 inches = 188cm<br />
                    </li>
                    <li>
                      과거진행형 : be과거형(was,were) + v-ing : 과거의 특정 시점을 전후해서 진행 중이던 일을 나타낼 때 사용되고 ~하고 있는 중이었다라고 해석합니다.<br />
                    </li>
                    <li>
                      과거진행형과 과거시제 : 과거진행형과 과거시제를 함께 쓸 때는 짧은 동작은 과거시제로, 긴 동작은 과거진행형으로 씁니다.<br />
                        Ex) I was walking to the parking lot when somebody hit me on the head : 누군가가 내 머리를 때렸을 때 나는 주차장을 걷고 있었다<br />                                 
                    </li>
                    <li>
                      every : 개별적인 것들의 전체를 가리키며, 원칙적으로 단수 취급합니다.<br />
                        every + 단수명사 : 모든 ~<br />
                    </li>
                    <li>
                      both : 복수취급을 합니다. both (of) + 복수명사 : 둘 다 <br />
                    </li>
                    <li>
                      quarter after nine : 9시 15분 (quarter는 1/4, after는 후)<br />
                    </li>
                    <li>
                      I'm not really sure : 정확히 모르겠다<br />
                    </li>
                    <li>
                      break one's leg : ~의 다리를 부러뜨리다<br />
                    </li>
                    <li>
                      He was attacked from behind : 그는 뒤로부터 공격받았다<br />
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
          name:'Police Officer:',
          speech:'What can you remember about the attack, Mr. Shaw?'
        },
        {
          name:'Mr. Shaw:',
          speech:'Well, I was working late last night.!'
        },
        {
          name:'Police Officer:',
          speech:'What time did you leave your office?'
        },
        {
          name:'Mr. Shaw:',
          speech:'At about a quarter after nine.'
        },
        {
          name:'Police Officer:',
          speech:'Are you sure?'
        },
        {
          name:'Mr. Shaw:',
          speech:'Yes, I am. I looked at my watch.'
        },
        {
          name:'Police Officer:',
          speech:'What did you do then?'
        },
        {
          name:'Mr. Shaw:',
          speech:'Well, I locked the office door, and I was walking to the parking lot when somebody hit me on the head.'
        },
        {
          name:'Police Officer:',
          speech:'Did you see the attacker?'
        },
        {
          name:'Mr. Shaw:',
          speech:'No. He was wearing a mask over his face.'
        },
        {
          name:'Police Officer:',
          speech:'He? Oh, so it was a man!'
        },
        {
          name:'Mr. Shaw:',
          speech:'Well, I’m not really sure. No… no, I don’t know'
        },
        {
          name:'Police Officer:',
          speech:'Tell me, Mr. Shaw, how did you break your leg?'
        },
        {
          name:'Mr. Shaw:',
          speech:'Yes. Her name’s Alicia, and she’s gorgeous!Well, when they were putting me into the ambulance, they dropped me!'
        },
        ],

        translations:[
        {
          name:'경찰관:',
          speech:'그 공격에 대해 기억나는 게 뭐죠, Shaw 씨?'
        },
        {
          name:'Mr. Shaw:',
          speech:'음, 어젯밤에 늦게까지 일하고 있었어요.'
        },
        {
          name:'경찰관:',
          speech:'몇 시에 퇴근했어요?'
        },
        {
          name:'Mr. Shaw:',
          speech:'9시 15분쯤에요.'
        },
        {
          name:'경찰관:',
          speech:'정말이에요?'
        },
        {
          name:'Mr. Shaw:',
          speech:'네, 그렇습니다. 나는 내 시계를 보았습니다.'
        },
        {
          name:'경찰관:',
          speech:'그때 당신은 무엇을 했습니까?'
        },
        {
          name:'Mr. Shaw:',
          speech:'음, 사무실 문을 잠그고 주차장으로 걸어가다가 누군가 제 머리를 때렸어요.'
        },
        {
          name:'경찰관:',
          speech:'당신은 그 공격자를 보았나요?'
        },
        {
          name:'Mr. Shaw:',
          speech:'아니요. 그는 얼굴에 마스크를 쓰고 있었습니다.'
        },
        {
          name:'경찰관:',
          speech:'그 사람요? 아, 그럼 남자였군요!'
        },
        {
          name:'Mr. Shaw:',
          speech:'글쎄, 잘 모르겠어요. 아뇨, 모르겠어요.'
        },
        {
          name:'경찰관:',
          speech:'말해봐요, Shaw씨, 어떻게 다리가 부러졌죠?'
        },
        {
          name:'Mr. Shaw:',
          speech:'음, 그들이 저를 구급차에 태울 때, 그들은 저를 내려줬어요!'
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
