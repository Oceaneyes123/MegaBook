<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/handsome-senior-man-holding-tablet_23-2148404383.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Man of the Year
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Man of the Year</li><br />

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

        <p>
          Look at the pictures, make conversations using the following words:<br />
          <br />
          successful / energetic / relaxed / ambitious / sociable / intelligent / polite<br />
        </p>
        <br />
        <p>
          Example:<br />
              A: Who’s more successful, Sam or Mr. Thompson?<br />
              B: Mr. Thompson is.<br />
              A: You’re right   OR   You’re wrong. Sam’s more successful.<br />
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
                      friend of yours : 너의 친구 / friend of mine : 나의 친구
                    </li>
                    <li>
                      Sam has more friends than anyone else : Sam은 어느 누구보다 더 많은 친구가 있다.
                    </li>
                    <li>
                      - generous with : ~에 관대한
                    </li>
                    <li>
                      he worked as a volunteer : 그는 자원봉사자로 일했다.
                    </li>
                    <li>
                      make a decision : 결정을 내리다
                    </li>
                    <li>
                      Man of the Year : 올해의 인물
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
          speech:'You know Sam Brown and Mr. Thompson, don’t you? They’re good friends of yours, aren’t they?'
        },
        {
          name:'B:',
          speech:'That’s right. All of us belong to the Lions Club.'
        },
        {
          name:'A:',
          speech:'Do you think Mr. Thompson is more successful than Sam?'
        },
        {
          name:'B:',
          speech:'That’s a difficult question. Both men are good at their jobs.'
        },
        {
          name:'A:',
          speech:'Well, which one is more hardworking?'
        },
        {
          name:'B:',
          speech:'I don’t know. They both work very hard.'
        },
        {
          name:'A:',
          speech:'Do you think Sam is more popular than Mr. Thompson?'
        },
        {
          name:'B:',
          speech:'Sure. Sam has more friends than anyone else in town.'
        },
        {
          name:'A:',
          speech:'But Mr. Thompson is more generous than Sam, isn’t he?'
        },
        {
          name:'B:',
          speech:'Only with his money.'
        },
        {
          name:'A:',
          speech:'You mean Sam is more generous with his time?'
        },
        {
          name:'B:',
          speech:'That’s right. Last year he worked as a volunteer for the Fire Department.'
        },
        {
          name:'A:',
          speech:'That’s interesting. Well, thanks for the information.'
        },
        {
          name:'B:',
          speech:'Wait a minute. Why are you asking all these questions?'
        },
        {
          name:'A:',
          speech:'So we can make a decision. We’re trying to decide who will be the next Man of the Year.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'Sam Brown 씨와 Thompson씨를 아시죠? 그들은 당신들의 좋은 친구죠, 그렇죠?'
        },
        {
          name:'B:',
          speech:'맞아요. 우리 모두는 라이온즈 클럽에 속해 있습니다.'
        },
        {
          name:'A:',
          speech:'맞아요. 우리 모두는 라이온즈 클럽에 속해 있습니다.'
        },
        {
          name:'B:',
          speech:'어려운 질문이네요. 두 사람 다 일을 잘해요.'
        },
        {
          name:'A:',
          speech:'음, 어느 쪽이 더 열심히 일하나요?'
        },
        {
          name:'B:',
          speech:'모르겠어요. 그들은 둘 다 매우 열심히 일합니다.'
        },
        {
          name:'A:',
          speech:'Sam 이 Thompson씨보다 더 인기가 있다고 생각하세요?'
        },
        {
          name:'B:',
          speech:'물론이죠. Sam 은 마을에 다른 누구보다도 많은 친구들을 가지고 있습니다.'
        },
        {
          name:'A:',
          speech:'하지만 Thompson씨는 Sam 보다 더 관대하죠?'
        },
        {
          name:'B:',
          speech:'돈만 가지고요.'
        },
        {
          name:'A:',
          speech:'Sam 이 시간을 더 많이 내준다는 말인가요?'
        },
        {
          name:'B:',
          speech:'맞아요. 작년에 그는 소방서에서 자원봉사자로 일했습니다.'
        },
        {
          name:'A:',
          speech:'흥미롭군요. 네, 알려주셔서 감사합니다.'
        },
        {
          name:'B:',
          speech:'잠깐만요. 왜 이런 질문을 하는 거죠?'
        },
        {
          name:'A:',
          speech:'그럼 결정을 내릴 수 있겠군요. 우리는 누가 올해의 인물이 될 것인지를 결정하려고 노력하고 있습니다.'
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
