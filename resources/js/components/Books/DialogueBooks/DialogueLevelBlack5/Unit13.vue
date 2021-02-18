<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/surgeons-performing-operation-operation-room_1170-2224.jpg" class="cover-photo">

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
        padding-bottom: 10px;">General Hospital
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">General Hospital</li><br />
      <br/>

      <p>
        Maternity Unit<br />
        Mr. Diaz is in the maternity unit. His wife's going to have a baby.<br />
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="mudialog in mudialogs" :key="mudialog">
          <td class = "uppertable" >{{mudialog.name}}</td>
          <td class = "lowertable" >{{mudialog.speech}}</td>
        </tr>
  
      </table>
      <br />
      <p>
        Operating Room<br />
        David Foster has had a serious accident. His wife's outside the operating room now.<br />
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="ordialog in ordialogs" :key="ordialog">
          <td class = "uppertable" >{{ordialog.name}}</td>
          <td class = "lowertable" >{{ordialog.speech}}</td>
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
          <u>Make sentences</u><br />
          Ex) We/operate/be all right   >   If we operate, he’ll be all right.<br />
        </p>

        <ol style="margin: 12px;">
          <li>
            You/not eat/not get well
          </li>
          <li>
            You/eat too much/get sick
          </li>
          <li>
            She/have a boy/call/Shawn
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
          산부인과<br />
          Diaz씨는 산부인과에 있습니다. 그의 아내가 아기를 낳을 거예요.<br />
        </p>
        <br />
        <table style = "border-collapse: collapse;">

        <tr v-for="mutranslation in mutranslations" :key="mutranslation">
          <td class = "uppertable" >{{mutranslation.name}}</td>
          <td class = "lowertable" >{{mutranslation.speech}}</td>
        </tr>

      </table>
      <br />
      <p>
        수술실<br />
        David Foster가 심각한 사고를 당했어요. 그의 아내는 지금 수술실 밖에 있어요.<br />
      </p>
      <br />
      <table style = "border-collapse: collapse;">

        <tr v-for="ortranslation in ortranslations" :key="ortranslation">
          <td class = "uppertable" >{{ortranslation.name}}</td>
          <td class = "lowertable" >{{ortranslation.speech}}</td>
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
                      be going to have a baby : 아기를 낳을 예정이다<br />
                    </li>
                    <li>
                      Have you been waiting long? : 오래 기다렸습니까? <br />
                    </li>
                    <li>
                      as soon as ~ : ~하자 마자
                    </li>
                    <li>
                      Have you thought of any names for the baby? : 아기 이름에 대해 생각해 보셨습니까?
                    </li>
                    <li>
                      have an accident : 사고나다
                    </li>
                    <li>
                      be afraid of ~ : ~을 두려워하다 (He's always been afraid of operations : 그는 항상 수술을 두려워했다)
                    </li>
                    <li>
                      He has lost a lot of blood : 그는 많은 피를 흘렸습니다
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
        mudialogs:[
        {
          name:'Nurse:',
          speech:'Hello. You’re Mr. Diaz, aren’t you? Have you been waiting long?'
        },
        {
          name:'Mr. Diaz:',
          speech:'Not really. Is there any news?'
        },
        {
          name:'Nurse:',
          speech:'Not yet. We’ll tell you as soon as there is. Have you thought of any names for the baby?'
        },
        {
          name:'Mr. Diaz:',
          speech:'Oh, yes. If it’s a girl, we’ll call her Lucia, and if it’s a boy we’ll call him Francisco.'
        },
        ],

        ordialogs:[
        {
          name:'Doctor:',
          speech:'Mrs. Foster? I’m Dr. Yamamura.'
        },
        {
          name:'Mrs. Foster:',
          speech:'Oh, doctor, how is he?'
        },
        {
          name:'Doctor:',
          speech:'Well, I’m afraid we’ll have to operate.'
        },
        {
          name:'Mrs. Foster:',
          speech:'Oh, no! He’s always been afraid of operations.'
        },
        {
          name:'Doctor:',
          speech:'Don’t worry. If we operate now, he’ll be all right.'
        },
        {
          name:'Mrs. Foster:',
          speech:'Oh, doctor, do you really have to?'
        },
        {
          name:'Doctor:',
          speech:'I’m afraid so. He’s lost a lot of blood. If we don’t operate, he’ll die!'
        },
        ],

        mutranslations:[
        {
          name:'간호사:',
          speech:'안녕하세요. Diaz 씨 맞죠? 오래 기다렸어요?'
        },
        {
          name:'Diaz 씨:',
          speech:'그렇진 않아요. 무슨 소식 있어요?'
        },
        {
          name:'간호사:',
          speech:'아직요. 거기에서 바로 이야기해 드릴게요. 생각해 본 적 있어요? 아기 이름은요?'
        },
        {
          name:'Diaz 씨:',
          speech:'아 네, 여자라면 Lucia라고 부르고, 남자라면 Francisco라고 부르죠.'
        },
        ],

        ortranslations:[
        {
          name:'의사:',
          speech:'Foster 부인요? Yamamura 박사입니다.'
        },
        {
          name:'Foster 부인:',
          speech:'오, 의사 선생님, 그는 어때요?'
        },
        {
          name:'의사:',
          speech:'음, 아무래도 수술을 해야 할 것 같아요.'
        },
        {
          name:'Foster 부인:',
          speech:'오, 안돼요! 그 사람은 전부터 항상 수술을 두려워했어요.'
        },
        {
          name:'의사:',
          speech:'걱정하지 마세요. 지금 수술하면 괜찮을 거예요'
        },
        {
          name:'Foster 부인:',
          speech:'아, 선생님, 정말 그렇게 해야 하나요?'
        },
        {
          name:'의사:',
          speech:'유감이지만 그렇습니다. 피를 많이 흘렸어요 지금 수술하지 않으면 그는 죽어요.'
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
