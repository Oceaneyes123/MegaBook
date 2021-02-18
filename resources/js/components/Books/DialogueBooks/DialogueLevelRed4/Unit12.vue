<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/dissatisfied-young-male-manager-looking-with-bugged-eyes-astonishment-shocked-by-financial-report-leaning-elbows-while-sitting-table-front-computer-screen-during-hard-working-day_176420-14542.jpg" class="cover-photo">

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
        padding-bottom: 10px;">What's the problem?
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">What's the problem?</li><br />
      <br />
      <p>
        1
      </p>
      <br />

      <table style = "border-collapse: collapse;">
    
        <tr v-for="firstdialog in firstdialogs" :key="firstdialog">
          <td class = "uppertable" >{{firstdialog.name}}</td>
          <td class = "lowertable" >{{firstdialog.speech}}</td>
        </tr>
  
      </table>
      <br />
      <p>
        2
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="seconddialog in seconddialogs" :key="seconddialog">
          <td class = "uppertable" >{{seconddialog.name}}</td>
          <td class = "lowertable" >{{seconddialog.speech}}</td>
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
          <u>Give advice - make sentences with should and shouldn’t</u><br />
        </p>
        <br />
        <p>
          Ex) Someone wants to become a doctor. > You should study day and night. It's going to be hard, but you shouldn't give up.<br />
        </p>
        <br />
        <ol style="margin: 12px;">
          <li>
            Your friend wants to lose weight. <br />
          </li>
          <li>
            Someone wants to learn Korean language. <br />
          </li>
          <li>
            Someone wants to learn Korean language. <br />
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
          1
        </p>
        <br />
        <table style = "border-collapse: collapse;">

          <tr v-for="firsttranslation in firsttranslations" :key="firsttranslation">
            <td class = "uppertable" >{{firsttranslation.name}}</td>
            <td class = "lowertable" >{{firsttranslation.speech}}</td>
          </tr>
  
        </table>
        <br />
        <p>
          2
        </p>
        <br />
        <table style = "border-collapse: collapse;">

          <tr v-for="secondtranslation in secondtranslations" :key="secondtranslation">
            <td class = "uppertable" >{{secondtranslation.name}}</td>
            <td class = "lowertable" >{{secondtranslation.speech}}</td>
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
                      to부정사 : It's hard to meet Americans -> To meet Americans is hard <br />
                    </li>
                    <li>
                      What's the matter? : 무슨 일이니? <br />
                    </li>
                    <li>
                      be worried about : ~을 걱정하다 <br />
                    </li>
                    <li>
                      I'm not practicing enough : 연습이 부족하다 <br />
                    </li>
                    <li>
                      take a class : 수강하다 <br />
                    </li>
                    <li>
                      be interested in : ~에 관심 있다 <br />
                    </li>
                    <li>
                      take a few days off : 며칠 쉬다 <br />
                    </li>
                    <li>
                      kill oneself : 자살하다 <br />
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
        firstdialogs:[
        {
          name:'Yoko:',
          speech:'What’s the matter, Dario? You’re very quiet today.'
        },
        {
          name:'Dario:',
          speech:'I’m worried about my English.'
        },
        {
          name:'Yoko:',
          speech:'What’s the problem?'
        },
        {
          name:'Dario:',
          speech:'I’m not practicing enough.'
        },
        {
          name:'Yoko:',
          speech:'Why not?'
        },
        {
          name:'Dario:',
          speech:'Well, it’s hard to meet Americans.'
        },
        {
          name:'Yoko:',
          speech:'You should go out more.'
        },
        {
          name:'Dario:',
          speech:'Where should I go?'
        },
        {
          name:'Yoko:',
          speech:'Maybe you should join a gym or take a class.'
        },
        {
          name:'Dario:',
          speech:'Americans never speak to me.'
        },
        {
          name:'Yoko:',
          speech:'Well, you should speak first.'
        },
        {
          name:'Dario:',
          speech:'What can I talk about?'
        },
        {
          name:'Yoko:',
          speech:'Sports! They’re always interested in sports!'
        },
        ],

        seconddialogs:[
        {
          name:'Karen:',
          speech:'Hello, Brian. You look tired today.'
        },
        {
          name:'Brian:',
          speech:'Yes, I’m working too hard.'
        },
        {
          name:'Karen:',
          speech:'You should take a few days off.'
        },
        {
          name:'Brian:',
          speech:'I know I should, but we’re just too busy. I’m working twelve hours a day.'
        },
        {
          name:'Karen:',
          speech:'Twelve hours a day! You’re going to kill yourself!'
        },
        {
          name:'Brian:',
          speech:'What else can I do?'
        },
        {
          name:'Karen:',
          speech:'Maybe you should quit the job.'
        },
        {
          name:'Brian:',
          speech:'I can’t. I need the money.'
        },
        ],

        firsttranslations:[
        {
          name:'Yoko:',
          speech:'Dario 씨, 왜 그래요? 당신은 오늘 매우 조용하군요.'
        },
        {
          name:'Dario:',
          speech:'제 영어 실력이 걱정돼요.'
        },
        {
          name:'Yoko:',
          speech:'뭐가 문제죠?'
        },
        {
          name:'Dario:',
          speech:'저는 충분히 연습하지 않고 있어요.'
        },
        {
          name:'Yoko:',
          speech:'왜 안되죠?'
        },
        {
          name:'Dario:',
          speech:'음, 미국인들을 만나는 것은 어렵습니다.'
        },
        {
          name:'Yoko:',
          speech:'더 나가셔야 해요.'
        },
        {
          name:'Dario:',
          speech:'어디로 가야 하나요?'
        },
        {
          name:'Yoko:',
          speech:'체육관에 들어가거나 수업을 듣는 게 좋겠어요.'
        },
        {
          name:'Dario:',
          speech:'미국인들은 제게 말을 걸지 않습니다.'
        },
        {
          name:'Yoko:',
          speech:'그럼, 먼저 말씀하세요.'
        },
        {
          name:'Dario:',
          speech:'제가 무슨 이야기를 할 수 있을까요?'
        },
        {
          name:'Yoko:',
          speech:'스포츠요! 그들은 항상 스포츠에 관심이 있어요!'
        },
        ],

        secondtranslations:[
        {
          name:'Karen:',
          speech:'안녕하세요, Brian. 당신 오늘 피곤해 보여요.'
        },
        {
          name:'Brian:',
          speech:'네, 저는 너무 열심히 일하고 있어요.'
        },
        {
          name:'Karen:',
          speech:'며칠 쉬셔야 해요.'
        },
        {
          name:'Brian:',
          speech:'그래야 한다는 건 알지만, 우리는 너무 바빠요. 저는 하루에 12시간 일하고 있어요.'
        },
        {
          name:'Karen:',
          speech:'하루에 12시간입니다! 당신은 자살할 거예요!'
        },
        {
          name:'Brian:',
          speech:'제가 또 무엇을 할 수 있을까요?'
        },
        {
          name:'Karen:',
          speech:'아마도 당신은 그 일을 그만두는 게 좋겠어요.'
        },
        {
          name:'Brian:',
          speech:'그럴 수 없어요. 나는 그 돈이 필요해요.'
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
