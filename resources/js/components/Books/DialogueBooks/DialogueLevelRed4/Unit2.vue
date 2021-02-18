<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/couple-with-luggage-reading-map_1398-4668.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Heavy suitcase
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

    <li style="list-style-type: none;">Heavy suitcase</li><br />

    <br />
    <p>
      In the hotel coffee shop (7:30 PM)<br />
    </p>
    <br />
    <table style = "border-collapse: collapse;">
    
      <tr v-for="firstdialog in firstdialogs"  :key="firstdialog">
        <td class = "uppertable" >{{firstdialog.name}}</td>
        <td class = "lowertable" >{{firstdialog.speech}}</td>
      </tr>

    </table>

    <br />
    <p>
      At the airport (8:00 PM)<br />
    </p>
    <br />
    <table style = "border-collapse: collapse;">
    
      <tr v-for="seconddialog in seconddialogs"  :key="seconddialog">
        <td class = "uppertable" >{{seconddialog.name}}</td>
        <td class = "lowertable" >{{seconddialog.speech}}</td>
      </tr>

    </table>

    <br />
    <p>
      At their destination(11:00 PM)<br />
    </p>
    <br />
    <table style = "border-collapse: collapse;">
    
      <tr v-for="thirddialog in thirddialogs"  :key="thirddialog">
        <td class = "uppertable" >{{thirddialog.name}}</td>
        <td class = "lowertable" >{{thirddialog.speech}}</td>
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
          Ex) He can’t lift it. It’s very heavy.   >   It’s too heavy for him to lift.<br />
        </p>

        <ol style="margin: 12px;">
          <li>
            They can’t drink it. It’s very hot.   >   <br />
          </li>
          <li>
            She can’t buy it. It’s too expensive.   >   <br />
          </li>
          <li>
            I can’t answer it. It’s very hard.    >   <br />
          </li>
          <li>
            We can’t see it. It’s very small.    >   <br />
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
          호텔 커피숍에서 (오후 7시 30분)<br />
        </p>
        <br />
        <table style = "border-collapse: collapse;">

          <tr v-for="firsttranslation in firsttranslations"  :key="firsttranslation">
            <td class = "uppertable" >{{firsttranslation.name}}</td>
            <td class = "lowertable" >{{firsttranslation.speech}}</td>
          </tr>
  
        </table>
        <br />
        <p>
          공항에서(오후 8시).<br />
        </p>
        <br />
        <table style = "border-collapse: collapse;">

          <tr v-for="secondtranslation in secondtranslations"  :key="secondtranslation">
            <td class = "uppertable" >{{secondtranslation.name}}</td>
            <td class = "lowertable" >{{secondtranslation.speech}}</td>
          </tr>
  
        </table>
        <br />
        <p>
          목적지(오후 11시)에 도착합니다.<br />
        </p>
        <br />
        <table style = "border-collapse: collapse;">

          <tr v-for="thirdtranslation in thirdtranslations"  :key="thirdtranslation">
            <td class = "uppertable" >{{thirdtranslation.name}}</td>
            <td class = "lowertable" >{{thirdtranslation.speech}}</td>
          </tr>
  
        </table>
        <br />

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
                      to부정사 : 형용사 + enough + to부정사 : ~할 정도로 충분히 ~한<br />
                            too + 형용사 + to부정사 : 너무 ~해서 ~할 수 없다<br />
                        <br />
                          Ex) This coffee's too hot for me to drink : 이 커피는 너무 뜨거워서 나는 마실 수 없다<br />
                            Is it cool enough for you to drink now? : 그것은 지금 너가 마시기에 충분히 차니?<br />
                            they're too heavy for me to carry : 그것들은 너무 무거워서 내가 운반할 수 없다<br />
                            I'm not strong enough to help you : 나는 너를 도와줄만큼 충분히 강하지 않다<br />
                            That's too far for me to walk : 너무 멀어서 걸을 수 없다<br />
                            We aren't rich enough to go everywhere by taxi : 택시로 어디든지 갈만큼 우리는 충분히 부유하지 않다<br />
                    </li>
                    <li>
                      to catch a taxi (bus, train, ...) : 택시를 잡다 <br />
                    </li>
                    <li>
                      to finish one's coffee (lunch, ...) : 커피마시는 것을 끝내라. <br />
                    </li>
                    <li>
                      he managed to carry the suitcase : 그는 짐을 옮겼다. <br />
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
          name:'Mike:',
          speech:'Come on, Kim. Hurry up and finish your coffee. We have to catch a taxi to the airport. We’ll be late.'
        },
        {
          name:'Kim:',
          speech:'I can’t hurry. This coffee’s too hot for me to drink.'
        },
        {
          name:'Mike:',
          speech:'Why don’t you put some cold milk in it?'
        },
        {
          name:'Kim:',
          speech:'Milk? I don’t take milk in my coffee. Oh, OK, OK.'
        },
        {
          name:'Mike:',
          speech:'Is it cool enough for you to drink now?'
        },
        {
          name:'Kim:',
          speech:'Yes, but it tastes awful!'
        },
        ],

        seconddialogs:[
        {
          name:'Kim:',
          speech:'Oh, no! The Global counter looks a mile away!'
        },
        {
          name:'Mike:',
          speech:'Ooh! What did you put in these suitcases? Rocks?'
        },
        {
          name:'Kim:',
          speech:'Only clothes. Why? Are they heavy?'
        },
        {
          name:'Mike:',
          speech:'Yes, they are.'
        },
        {
          name:'Kim:',
          speech:'The taxi driver managed to carry them.'
        },
        {
          name:'Mike:',
          speech:'Well, they’re too heavy for me to carry, and I don’t see any luggage carts.'
        },
        {
          name:'Kim:',
          speech:'Well, I’m not strong enough to help you. Porter! Over here, please.'
        },
        ],

        thirddialogs:[
        {
          name:'Kim:',
          speech:'Oh, no! There goes the last bus!'
        },
        {
          name:'Mike:',
          speech:'Well, let’s walk to the highway and catch a different bus.'
        },
        {
          name:'Kim:',
          speech:'It’s a mile away! That’s too far for me to walk. Let’s take a taxi.'
        },
        {
          name:'Mike:',
          speech:'Another taxi! We aren’t rich enough to go everywhere by taxi.'
        },
        {
          name:'Kim:',
          speech:'Mike, didn’t you forget something?'
        },
        {
          name:'Mike:',
          speech:'What?'
        },
        {
          name:'Kim:',
          speech:'We have three suitcases. Do you really want to walk?'
        },
        {
          name:'Mike:',
          speech:'You’re right. Taxi!'
        },
        ],

        firsttranslations:[
        {
          name:'Mike:',
          speech:'어서요, Kim . 빨리 커피를 마저 드세요. 공항까지 택시를 타야해요. 늦겠어요.'
        },
        {
          name:'Kim:',
          speech:'서두를 수가 없어요. 이 커피가 너무 뜨거워서 못 마시겠어요.'
        },
        {
          name:'Mike:',
          speech:'차가운 우유를 넣어보는 건 어때요?'
        },
        {
          name:'Kim:',
          speech:'우유요? 저는 제 커피에 우유를 넣지 않아요. 오, 알았어요, 알았어요.'
        },
        {
          name:'Mike:',
          speech:'지금 마실 수 있을 만큼 충분히 시원합니까?'
        },
        {
          name:'Kim:',
          speech:'네, 하지만 맛이 끔찍해요!'
        },
        ],

        secondtranslations:[
        {
          name:'Kim:',
          speech:'아, 안 돼요! 글로벌 카운터는 1마일 떨어져 있습니다!'
        },
        {
          name:'Mike:',
          speech:'오! 이 여행가방에 뭘 넣었어요? 돌이라고요?'
        },
        {
          name:'Kim:',
          speech:'옷만. 왜요? 그것들은 무겁습니까?'
        },
        {
          name:'Mike:',
          speech:'네, 그렇습니다.'
        },
        {
          name:'Kim:',
          speech:'택시 기사가 가까스로 이들을 실어 나릅니다.'
        },
        {
          name:'Mike:',
          speech:'음, 그것들은 제가 들고 다니기에는 너무 무겁고, 짐수레는 하나도 보이지 않아요.'
        },
        {
          name:'Kim:',
          speech:'저, 제가 힘이 없어서 도와드릴 수가 없어요. 포터요! 여기 주세요.'
        },
        ],

        thirdtranslations:[
        {
          name:'Kim:',
          speech:'아, 안 돼요! 저기 마지막 버스가 갑니다!'
        },
        {
          name:'Mike:',
          speech:'그럼, 고속도로로 걸어가서 다른 버스를 타죠.'
        },
        {
          name:'Kim:',
          speech:'1마일 떨어져 있어요! 거긴 너무 멀어서 못 걷겠어요. 택시를 타고 가죠.'
        },
        {
          name:'Mike:',
          speech:'택시 한 대 더요! 우리는 택시를 타고 어디든지 갈 만큼 부자가 아닙니다.'
        },
        {
          name:'Kim:',
          speech:'Mike, 뭐 잊은 거 없어요?'
        },
        {
          name:'Mike:',
          speech:'뭐라고요?'
        },
        {
          name:'Kim:',
          speech:'가방이 세 개 있습니다. 정말 걷고 싶어요?'
        },
        {
          name:'Mike:',
          speech:'맞아요. 택시!'
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
