<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/traveling-through-door-future-with-speed-light_41470-1637.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Invention
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Invention</li><br />

      <br />
      <p>
        Dr. Finkel is an inventor. He designed a new machine. The machine can change people. His assistant, Boris, is going to try the machine for the first time.<br />
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
            What can Dr. Finkel’s machine do?<br />
          </li>
          <li>
            What do you think Boris feels before trying the machine?<br />
          </li>
          <li>
            What happened to Boris after trying Dr. Finkel’s machine?<br />
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
          Finkel 박사는 발명가이다. 그는 새로운 기계를 디자인했습니다. 그 기계는 사람을 변화시킬 수 있습니다. 그의 조수인 Boris는 처음으로 그 기계를 시험해 볼 것입니다.
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
                      비교급 만들기 : 형용사나 부사가 2,3 음절 이상일 경우에는 비교급을 만들 때 er을 붙이지 않고 앞에 more나 less를 붙입니다.<br />                 
                    </li>
                    <li>
                      for the first time : 처음에
                    </li>
                    <li>
                      get into : 안으로 들어가다
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
          name:'Boris:',
          speech:'Is it safe, doctor?'
        },
        {
          name:'Finkel:',
          speech:'Oh, yes. Yes, of course it is, Boris.'
        },
        {
          name:'Boris:',
          speech:'I’m afraid, doctor.'
        },
        {
          name:'Finkel:',
          speech:'Nonsense! This machine is going to change you! You’re going to be a better person, Boris.'
        },
        {
          name:'Boris:',
          speech:'A better person?'
        },
        {
          name:'Finkel:',
          speech:'Yes! Stronger! Uh, thinner! Healthier! Happier!'
        },
        {
          name:'Boris:',
          speech:'I’m happy now, doctor.'
        },
        {
          name:'Finkel:',
          speech:'Well, you’re going to be happier. And more intelligent.'
        },
        {
          name:'Boris:',
          speech:'I’m intelligent now, doctor.'
        },
        {
          name:'Finkel:',
          speech:'Uh, yes. Well, you’re less intelligent than I am, Boris. Just get into the machine…'
        },
        {
          name:'Boris:',
          speech:'But doctor… ooh! Uh!… Wah! Wah!'
        },
        {
          name:'Finkel:',
          speech:'Hmm. Yes. And younger, too. Sorry about that, Boris.'
        },
        {
          name:'Boris:',
          speech:'Mommy! I want my mommy…'
        },
        ],

        translations:[
        {
          name:'Boris:',
          speech:'안전한가요, 박사님?'
        },
        {
          name:'Finkel:',
          speech:'아, 그래요. 네, 물론 그렇습니다. Boris.'
        },
        {
          name:'Boris:',
          speech:'유감입니다, 박사님.'
        },
        {
          name:'Finkel:',
          speech:'말도 안 돼요! 이 기계는 당신을 변화시킬 거예요! 당신은 더 나은 사람이 될 거예요, Boris.'
        },
        {
          name:'Boris:',
          speech:'더 나은 사람이요?'
        },
        {
          name:'Finkel:',
          speech:'네! 더 강하게! 더 날씬하게! 더 건강하게! 더 행복하게요!'
        },
        {
          name:'Boris:',
          speech:'박사님, 저는 지금 행복합니다.'
        },
        {
          name:'Finkel:',
          speech:'음, 당신은 더 행복해질 거예요. 그리고 더 똑똑해질 거예요.'
        },
        {
          name:'Boris:',
          speech:'저는 지금 똑똑해요, 박사님.'
        },
        {
          name:'Finkel:',
          speech:'어, 그래요. 저보다 지능이 떨어지는군요, Boris 그냥 기계에 들어가세요…'
        },
        {
          name:'Boris:',
          speech:'하지만 박사님은… 우! 어!… 와! 와! 와! 와! 와!'
        },
        {
          name:'Finkel:',
          speech:'흠. 그래요. 그리고 더 어려져요요. 미안해요, Boris.'
        },
        {
          name:'Boris:',
          speech:'엄마! 엄마 보고 싶어요'
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
