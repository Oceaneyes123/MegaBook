 <template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/multiracial-group-coworkers-laughing-together_23-2148222536.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Have you ever…?
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Have you ever…?</li><br />

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
            Have you ever learned how to play a musical instrument? When and what did you learn?
          </li>
          <li>
            Have you ever broken a bone?
          </li>
          <li>
            Have you ever been to a wedding? Whose wedding was it?
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
                      현재완료와 과거시제 : 과거시제는 현재와는 무관한 과거의 사실만을 말할 때 사용되고 현재완료는 과거에 대한 이야기를 하지만 결국 말하고자 하는 것은 현재의 상황일 때 사용됩니다.
                    </li>
                    <li>
                      Have you ever : ~한 적이 있습니까?
                    </li>
                    <li>
                      Have you ever been : ~에 가 본 적이 있습니까?
                    </li>
                    <li>
                      bad fire : 큰 불(심한불)
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
          speech:'Have you ever studied a language before?'
        },
        {
          name:'B:',
          speech:'Yes, I have.'
        },
        {
          name:'A:',
          speech:'Oh, which one did you study?'
        },
        {
          name:'B:',
          speech:'I studied Spanish in high school.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'Have you ever been to a big wedding?'
        },
        {
          name:'D:',
          speech:'Yes, I have.'
        },
        {
          name:'C:',
          speech:'Oh, which one did you study?'
        },
        {
          name:'D:',
          speech:'I studied Spanish in high school.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'Have you ever seen a fire?'
        },
        {
          name:'F:',
          speech:'Uh, yes, I have.'
        },
        {
          name:'E:',
          speech:'When did you see it?'
        },
        {
          name:'F:',
          speech:'I saw a bad fire in Detroit in 1992.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'G:',
          speech:'Have you ever eaten sushi?'
        },
        {
          name:'H:',
          speech:'Yes, I have.'
        },
        {
          name:'G:',
          speech:'Where did you eat it?'
        },
        {
          name:'H:',
          speech:'Maria and I ate sushi in Hawaii last year.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'I:',
          speech:'Have you ever had the flu?'
        },
        {
          name:'J:',
          speech:'Yes, I have.'
        },
        {
          name:'I:',
          speech:'When did you have it?'
        },
        {
          name:'J:',
          speech:'I had it last winter.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'K:',
          speech:'Have you ever broken a bone?'
        },
        {
          name:'L:',
          speech:'Yes, I have.'
        },
        {
          name:'K:',
          speech:'What did you break?'
        },
        {
          name:'L:',
          speech:'I broke my leg.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'전에 언어 공부해 본 적 있어?'
        },
        {
          name:'B:',
          speech:'응, 그랬어.'
        },
        {
          name:'A:',
          speech:'아, 어떤 걸 공부했니?'
        },
        {
          name:'B:',
          speech:'고등학교 때 스페인어를 공부했어.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'큰 결혼식에 가본 적 있어?'
        },
        {
          name:'D:',
          speech:'응, 그랬어.'
        },
        {
          name:'C:',
          speech:'누구의 결혼식이었니?'
        },
        {
          name:'D:',
          speech:'내 동생 거였어.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'화재 본 적 있어?'
        },
        {
          name:'F:',
          speech:'어, 그래, 있어.'
        },
        {
          name:'E:',
          speech:'언제 봤어?'
        },
        {
          name:'F:',
          speech:'1992년에 디트로이트에서 불이 난 걸 봤어.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'G:',
          speech:'초밥 먹어본 적 있어?'
        },
        {
          name:'H:',
          speech:'응, 그랬어.'
        },
        {
          name:'G:',
          speech:'어디서 먹었어?'
        },
        {
          name:'H:',
          speech:'Maria 와 나는 작년에 하와이에서 초밥을 먹었어.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'I:',
          speech:'독감에 걸린 적 있어?'
        },
        {
          name:'J:',
          speech:'응, 그랬어.'
        },
        {
          name:'I:',
          speech:'언제 먹었어?'
        },
        {
          name:'J:',
          speech:'작년 겨울에 먹었어.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'K:',
          speech:'뼈가 부러진 적 있어?'
        },
        {
          name:'L:',
          speech:'응, 있어.'
        },
        {
          name:'K:',
          speech:'뭘 부러뜨렸어?'
        },
        {
          name:'L:',
          speech:'다리가 부러졌어.'
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
