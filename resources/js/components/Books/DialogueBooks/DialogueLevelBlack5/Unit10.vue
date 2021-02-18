<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/cheerful-courier-car-smiling-camera_23-2147767603.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Big fan
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Big fan</li><br />
      <br />
      <p>
        Fred Barnes has been driving a taxi for several years. He enjoys his work because it gives him a chance to meet a lot of interesting people. Last week, for example, he met a famous movie star at the airport. It was Angela Joule, Fred’s favorite actress. He recognized her as soon as she got in the taxi.<br />
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
            Why does Angela think Fred is different from other people?<br />
          </li>
          <li>
            Why isn’t Fred afraid to talk to Angela?<br />
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
          Fred Barnes는 몇 년 동안 택시를 운전해 왔습니다. 그는 일을 즐깁니다. 왜냐하면 그것은 그에게 많은 흥미로운 사람들을 만날 기회를 주기 때문입니다. 예를 들어, 지난 주, 그는 공항에서 유명한 영화배우를 만났습니다. Fred 가 가장 좋아하는 여배우 안젤라 Joule이었어요. 그는 그녀가 택시에 오르자마자 그녀를 알아봤어요.<br />
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
                      "he has been driving a taxi for several years" : 그는 몇 년동안 택시를 운전하고 있습니다 <br />
                    </li>
                    <li>
                      "it gives him a chance to meet a lot of interesting people" : 그것은 그에게 많은 재미있는 사람들을 만날 기회를 줍니다<br />
                    </li>
                    <li>
                      as soon as : ~하자 마자<br />
                    </li>
                    <li>
                      you're quite a guy : 당신은 남자답습니다.
                    </li>
                    <li>
                      at a person's service : ~의 원하는대로, 마음대로
                    </li>
                    <li>
                      different from : ~와 다른
                    </li>
                    <li>
                      be afraid to + 동사원형 : ~하는 것을 두려워하다
                    </li>
                    <li>
                      seem to do : ~가 ~하는 것 같이 생각되다, ~하는 것 같은 느낌이 들다, ~하는 것 같이 여겨지다
                    </li>
                    <li>
                      seem like : ~처럼 보이다
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
          name:'Joule:',
          speech:'Please take me to the Plaza Hotel. And don’t waste any time.'
        },
        {
          name:'Fred:',
          speech:'Yes, ma’am. Aren’t you Miss Angela Joule, the famous actress?'
        },
        {
          name:'Joule:',
          speech:'That’s right. I suppose you’ve seen me in the movies.'
        },
        {
          name:'Fred:',
          speech:'I sure have. I’ve seen all of your pictures. I’m a real fan of yours.'
        },
        {
          name:'Joule:',
          speech:'Oh, really?'
        },
        {
          name:'Fred:',
          speech:'Yes, I really enjoy watching your movies. I think you’re the best actress in the world.'
        },
        {
          name:'Joule:',
          speech:'You’re just flattering me.'
        },
        {
          name:'Fred:',
          speech:'No, it’s true Miss Joule.'
        },
        {
          name:'Joule:',
          speech:'You’re quite a guy. What’s your name?'
        },
        {
          name:'Fred:',
          speech:'Fred Barnes. At your service.'
        },
        {
          name:'Joule:',
          speech:'You know, Fred, you’re different from most people I meet. Almost everyone is afraid to talk to me because I’m a big star. But it doesn’t seem to bother you at all.'
        },
        {
          name:'Fred:',
          speech:'Well, I am a little nervous. But in my work I meet all kinds of people, and I enjoy talking.'
        },
        {
          name:'Joule:',
          speech:'Don’t stop now. Tell me about yourself. You seem like a very interesting person.'
        },
        ],

        translations:[
        {
          name:'Joule:',
          speech:'플라자 호텔로 데려다 주세요. 그리고 시간을 낭비하지 마세요.'
        },
        {
          name:'Fred:',
          speech:'네, 부인. 당신이 유명한 여배우인 Angela Joule 아닌가요?'
        },
        {
          name:'Joule:',
          speech:'맞아요. 영화에서 절 보셨나 봐요.'
        },
        {
          name:'Fred:',
          speech:'물론 그랬죠. 당신의 사진을 다 봤어요. 저는 당신의 진정한 팬입니다.'
        },
        {
          name:'Joule:',
          speech:'아, 그래요?'
        },
        {
          name:'Fred:',
          speech:'네, 저는 정말 당신의 영화를 보는 것을 좋아해요. 당신이 세계 최고의 여배우라고 생각해요.'
        },
        {
          name:'Joule:',
          speech:'그냥 아첨하는 거예요.'
        },
        {
          name:'Fred:',
          speech:'아니요, 진짜 Joule 양입니다.'
        },
        {
          name:'Joule:',
          speech:'당신은 꽤 괜찮은 사람이에요. 성함이 어떻게 되세요?'
        },
        {
          name:'Fred:',
          speech:'반스입니다. 당신들 서비스에서요.'
        },
        {
          name:'Joule:',
          speech:'Fred , 당신은 내가 만나는 대부분의 사람들과 달라요. 거의 모든 사람들이 제가 대스타이기 때문에 저와 대화하는 것을 두려워합니다. 하지만 그것은 전혀 당신을 귀찮게 하지 않는 것 같습니다.'
        },
        {
          name:'Fred:',
          speech:'음, 저는 조금 긴장돼요. 하지만 제 작품에서 저는 모든 종류의 사람들을 만나고, 이야기하는 것을 즐깁니다.'
        },
        {
          name:'Joule:',
          speech:'지금 멈추지 마세요. 당신에 대해 말씀해주세요 당신은 매우 흥미로운 사람인 것 같아요.'
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
