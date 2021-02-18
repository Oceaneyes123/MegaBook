<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/beautiful-smart-asian-doctor-patient-discussing-explaining-something-with-clipboard_7861-1219.jpg" class="cover-photo">

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
        padding-bottom: 10px;">General Hospital II
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">General Hospital II</li><br />
      <p>
        East Wing<br />
        Ms. Wright has just arrived at the hospital. She's going to have a minor operation tomorrow.<br />
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="ewdialog in ewdialogs" :key="ewdialog">
          <td class = "uppertable" >{{ewdialog.name}}</td>
          <td class = "lowertable" >{{ewdialog.speech}}</td>
        </tr>
  
      </table>
      <br />
      <p>
        Emergency Room<br />
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="erdialog in erdialogs" :key="erdialog">
          <td class = "uppertable" >{{erdialog.name}}</td>
          <td class = "lowertable" >{{erdialog.speech}}</td>
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
          Ex) we/operate/be all right   >   If we operate, he’ll be all right.
        </p>

        <ol style="margin: 12px;">
          <li>
            you/take pills/feel better<br />
          </li>
          <li>
            he/press the buzzer/nurse/come<br />
          </li>
          <li>
            you/not take the medicine/not feel better<br />
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
          이스트 윙<br />
          Wright 양이 방금 병원에 도착했습니다. 그녀는 내일 경미한 수술을 받을 거예요.<br />
        </p>
        <br />
        <table style = "border-collapse: collapse;">

        <tr v-for="ewtranslation in ewtranslations" :key="ewtranslation">
          <td class = "uppertable" >{{ewtranslation.name}}</td>
          <td class = "lowertable" >{{ewtranslation.speech}}</td>
        </tr>

      </table>
      <br />
      <p>
        응급실<br />
      </p>
      <br />
      <table style = "border-collapse: collapse;">

        <tr v-for="ertranslation in ertranslations" :key="ertranslation">
          <td class = "uppertable" >{{ertranslation.name}}</td>
          <td class = "lowertable" >{{ertranslation.speech}}</td>
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
                      get undressed : 옷을 벗다<br />
                    </li>
                    <li>
                      press the button : 버튼을 누르다<br />
                    </li>
                    <li>
                      right away : 곧, 즉시, 당장에<br />
                    </li>
                    <li>
                      it's stuck : 걸렸다<br />
                    </li>
                    <li>
                      get off : 빼다, 벗다<br />
                    </li>
                    <li>
                      be afraid of doing : ~하기를 겁내는, ~하기를 주저하는<br />
                    </li>
                    <li>
                      come off easily: 쉽게 빠지다
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
      ewdialogs:[
        {
          name:'Nurse:',
          speech:'This is your bed, Ms. Wright.'
        },
        {
          name:'Ms. Wright:',
          speech:'Oh, thank you, nurse.'
        },
        {
          name:'Nurse:',
          speech:'Now, get undressed and get into bed. There’s a buzzer on the night table. If you press the button, someone will come right away.'
        },
        {
          name:'Ms. Wright:',
          speech:'Oh, I’m sure I won’t need anything.'
        },
        {
          name:'Nurse:',
          speech:'Well, don’t forget — if you need anything, just press the button.'
        },
        ],

        erdialogs:[
        {
          name:'Doctor:',
          speech:'Oh! How did this happen?'
        },
        {
          name:'Mother:',
          speech:'He was playing soldier, and he put the pot over his head. Now it’s stuck!'
        },
        {
          name:'Doctor:',
          speech:'Have you tried to get it off?'
        },
        {
          name:'Mother:',
          speech:'No, I’m afraid of hurting him.'
        },
        {
          name:'Doctor:',
          speech:'Yes, if we pull too hard, we’ll hurt him.'
        },
        {
          name:'Mother:',
          speech:'What are you going to do?'
        },
        {
          name:'Doctor:',
          speech:'Well, if I don’t get it off, he won’t be able to eat!'
        },
        {
          name:'Mother:',
          speech:'Oh, no!'
        },
        {
          name:'Doctor:',
          speech:'I’m only joking. If I put some soap on his head, it’ll come off easily.'
        },
        ],

        mutranslations:[
        {
          name:'간호사:',
          speech:'여기가 당신의 침대예요, Wright 양.'
        },
        {
          name:'Wright:',
          speech:'고마워요, 간호사님'
        },
        {
          name:'간호사:',
          speech:'자, 이제 옷을 벗고 침대로 들어가세요. 밤 테이블 위에 버저가 있습니다. 버튼을 누르면 바로 사람이 올 거예요.'
        },
        {
          name:'Wright:',
          speech:'아, 저는 아무 것도 필요 없을 거라고 확신해요.'
        },
        {
          name:'간호사:',
          speech:'음, 잊지 마세요. 필요한 게 있으면 버튼만 누르세요.'
        },
        ],

        ortranslations:[
        {
          name:'의사:',
          speech:'아! 어떻게 이런 일이 일어났죠?'
        },
        {
          name:'어머니:',
          speech:'군인놀이 하다가 냄비를 머리 위에 올려놓았어요. 갇혔어요!'
        },
        {
          name:'의사:',
          speech:'떼어내려고 노력했어요?'
        },
        {
          name:'어머니:',
          speech:'아니요, 그 사람을 해칠까 봐 두려워요.'
        },
        {
          name:'의사:',
          speech:'네, 너무 세게 당기면 다치게 됩니다.'
        },
        {
          name:'어머니:',
          speech:'어떻게 하실 거예요?'
        },
        {
          name:'의사:',
          speech:'음, 제가 그것을 벗지 못하면, 그는 먹을 수 없을 거예요!'
        },
        {
          name:'어머니:',
          speech:'아, 안돼요!'
        },
        {
          name:'의사:',
          speech:'농담입니다. 제가 그의 머리에 비누를 좀 발랐다면, 쉽게 벗겨질 거예요.'
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
