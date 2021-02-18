<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/beautiful-smart-asian-doctor-patient-discussing-explaining-something-with-tablet_7861-1234.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Recovery
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Recovery</li><br />

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
            When will Judy be able to move around?
          </li>
          <li>
            Will she ever be able to fly again
          </li>
          <li>
            Why will Judy need a new plane?
          </li>
        </ol>

        <p>
          Free response:<br />
            Have you ever been to a hospital?<br />
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
                      조동사 can :<br />
                          능력의 'can'은 'be able to'로 바꿀 수 있는데, 현재시제에서는 can을 더 많이 씁니다. can의 부정은 can't로 씁니다. <br />
                          과거의 능력에 있어서 실제로 그 일을 해낸 경우는 'was(were) able to'를 씁니다 이 때 could는 쓸 수 없습니다.<br />
                        could는 실제로 한 것은 아니고 마음만 먹으면 언제든지 할 수 있었다는 과거의 평상시 능력을 나타냅니다. <br />
                        미래의 능력은 'will be able to'로 나타냅니다. 조동사 will과 can은 연달아 같이 쓸 수 없기 때문입니다. <br />
                        <br />
                        Example:<br />
                            She wasn't able to receive any visitors : 그녀는 어떤 방문자도 받을 수 없었습니다. <br />
                            She won't be able to move around until next week : 다음 주까지 그녀는 주위를 돌아다닐 수 없을 것입니다. <br />
                            Will she be able to leave the hospital? : 그녀는 병원을 떠날 수 있을까요?<br />
                            She'll be able to fly in a few months : 그녀는 몇달안에 비행할 수 있을 것입니다. <br />               
                    </li>
                    <li>
                      to부정사의 부사적 용법 : 어떤 행동의 이유나 목적을 밝힐 때 사용합니다<br />
                          Example: I went to the hospital to see Judy : 나는 Judy를 만나기 위해 병원으로 갔습니다.<br />
                    </li>
                    <li>
                      get out of : ~에서 나오다<br />
                    </li>
                    <li>
                      "it must be boring to lie in bed all day" : 하루 종일 침대에 누워 있는 것은 지루할 것임에 틀림 없습니다<br />
                    </li>
                    <li>
                      how soon : 얼마의 시간이면
                    </li>
                    <li>
                      "it depends on how fast she recovers" : 얼마나 빨리 회복되느냐에 달려 있습니다
                    </li>
                    <li>
                      "Do you think she’ll ever fly again?" : 그녀가 언젠가 다시 비행할 수 있을 거라 생각하니?
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
          speech:'Where were you yesterday afternoon? I was trying to find you.'
        },
        {
          name:'B:',
          speech:'I went to the hospital to see Judy.'
        },
        {
          name:'A:',
          speech:'How is she doing?'
        },
        {
          name:'B:',
          speech:'Much better. At first she wasn’t able to receive any visitors except family members. Now she can see anyone she wants.'
        },
        {
          name:'A:',
          speech:'Can she get out of bed and move around?'
        },
        {
          name:'B:',
          speech:'No, it’s still too early. She won’t be able to move around until next week.'
        },
        {
          name:'A:',
          speech:'I feel sorry for her. It must be boring to lie in bed all day.'
        },
        {
          name:'B:',
          speech:'It isn’t too bad. At least she can sit up and watch television. And she does a lot of reading.'
        },
        {
          name:'A:',
          speech:'How soon will she be able to leave the hospital?'
        },
        {
          name:'B:',
          speech:'I don’t know. It depends on how fast she recovers.'
        },
        {
          name:'A:',
          speech:'Do you think she’ll ever fly again?'
        },
        {
          name:'B:',
          speech:'Yes. She’ll be able to fly in a few months. But she’ll need a new airplane. That’s for sure. The old one is completely destroyed.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'어제 오후에 어디 있었어요? 당신을 찾으려고 했어요.'
        },
        {
          name:'B:',
          speech:'Judy를 보러 병원에 갔어요.'
        },
        {
          name:'A:',
          speech:'그녀는 어때요?'
        },
        {
          name:'B:',
          speech:'훨씬 낫습니다. 처음에 그녀는 가족 외에는 어떤 방문객도 받을 수 없었는데 이제 그녀는 원하는 사람을 볼 수 있습니다.'
        },
        {
          name:'A:',
          speech:'침대에서 일어나서 돌아다닐 수 있을까요?'
        },
        {
          name:'B:',
          speech:'아니요, 아직 너무 일러요. 그녀는 다음 주까지 움직일 수 없을 거예요.'
        },
        {
          name:'A:',
          speech:'그녀가 불쌍해요. 하루 종일 침대에 누워있으니 지루하겠어요'
        },
        {
          name:'B:',
          speech:'그렇게 나쁘진 않아요. 적어도 그녀는 앉아서 텔레비전을 볼 수 있어요. 그리고 그녀는 독서를 많이 합니다.'
        },
        {
          name:'A:',
          speech:'언제쯤 퇴원할 수 있을까요?'
        },
        {
          name:'B:',
          speech:'모르겠어요. 그녀가 얼마나 빨리 회복하느냐에 달렸어요.'
        },
        {
          name:'A:',
          speech:'그녀가 다시 날 수 있을까요?'
        },
        {
          name:'B:',
          speech:'네. 몇 달 후면 비행기를 탈 수 있을 거예요. 하지만 새 비행기가 필요할 거예요. 그건 확실해요. 낡은 것이 완전히 파괴되었습니다.'
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
