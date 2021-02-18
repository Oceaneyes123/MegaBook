<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/suit-landing-astronaut-walk-moon_121-60616.jpg" class="cover-photo">

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
        padding-bottom: 10px;">On the moon
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">On the moon</li><br />

      <p>
        The Eagle has landed on the moon! Astronaut Phil Strongarm is speaking to Mission Control in Houston.
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

          <v-container grid-list-md text-xs-center>
            <v-layout wrap align-content-center>
  
              <v-flex xs12 md4 >
                <v-card hover>
  
                  <v-img src="images/kfcmap.gif" />
  
                </v-card>
              </v-flex>
  
            </v-layout>
          </v-container>

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
          독수리가 달에 착륙했습니다! 우주비행사 Phil Strongarm이 휴스턴에 있는 관제 센터와 통화하고 있습니다.<br />
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
                      현재완료 : 과거의 어느 한 시점에서 일어난 일 뿐만 아니라 과거의 일이 현재까지 영향을 미쳐 현재와 관련이 있을 때 사용합니다.<br />
                          형태는 have(has) + 과거분사 (과거분사: 동사원형 +ed, 명사를 수식하는 경우 수동의 의미를 나타내 ~된, ~받는 등으로 해석됨)<br />
                              *open > have opened<br />
                              *raise > have raised<br />           
                              Irregular:    do    >     have done <br />
                    </li>
                    <li>
                      현재진행형 : 현재진행되고 있는 행동이나 앞으로 예정되어 있는 가까운 미래의 일을 표현할 때 사용합니다. 형태는 be(is,are) +v-ing<br />
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
          name:'Mission Control:',
          speech:'Hello, Phil. Can you hear me?'
        },
        {
          name:'Strongarm:',
          speech:'Yes, I can hear you clearly.'
        },
        {
          name:'Mission Control:',
          speech:'What are you going to do next?'
        },
        {
          name:'Strongarm:',
          speech:'I’m going to open the door.'
        },
        {
          name:'Mission Control:',
          speech:'Hello, Phil. What are you doing now?'
        },
        {
          name:'Strongarm:',
          speech:'I’m opening the door.'
        },
        {
          name:'Mission Control:',
          speech:'Phil! Have you opened the door?'
        },
        {
          name:'Strongarm:',
          speech:'Yes, I’ve opened it! I can see the moon, and it’s fantastic!'
        },
        ],

        translations:[
        {
          name:'관제 센터:',
          speech:'안녕하세요, 필 내 말 들려요?'
        },
        {
          name:'Strongarm:',
          speech:'네, 잘 들리네요.'
        },
        {
          name:'관제 센터:',
          speech:'다음엔 뭘 할 거예요?'
        },
        {
          name:'Strongarm:',
          speech:'문을 열려고 합니다.'
        },
        {
          name:'관제 센터:',
          speech:'안녕하세요, Phil 당신은 지금 무엇을 하고 있나요?'
        },
        {
          name:'Strongarm:',
          speech:'문을 열고 있어요.'
        },
        {
          name:'관제 센터:',
          speech:'필, 문 열었어요?'
        },
        {
          name:'Strongarm:',
          speech:'네, 열었어요! 달도 보이고 환상적이에요!'
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
