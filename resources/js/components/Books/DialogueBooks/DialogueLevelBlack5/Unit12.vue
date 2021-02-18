<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/uncertain-woman-standing-with-raised-hands-aside-shrugging-shoulders-having-courage-make-decision-young-housewife-wearing-yellow-raincoat-going-have-walk-outdoors-rainy-weather_273609-8068.jpg" class="cover-photo">

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
        padding-bottom: 10px;">What if it rains?
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">What if it rains?</li><br />
      
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
          Talk about your plans for Sunday<br />
        </p>
        <br />
        <p>
          Example: <br />
            A: What are you going to do on Sunday?<br />
            B: Well, if it’s a nice day, I’ll …<br />
            A: What if it rains?<br />
            B: If it rains, I’ll …<br />

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
                      조건,양보를 나타내는 접속사 : if (만약 ~한다면) / unless (만약 ~하지 않는다면)<br />
                    </li>
                    <li>
                      현재시제가 미래의 뜻을 나타내는 경우 : 때나 조건을 나타내는 부사절에서는 미래의 일이라도 현재시제를 사용합니다<br />
                          Example:<br />
                            If it’s a nice day, I’ll go fishing at Beat Lake : 만약 날씨가 좋다면 나는 Beat Lake로 낚시하러 갈 것이다 (조건)<br />
                            If it rains, I’ll stay home and paint the living room : 만약 비가 온다면 나는 집에 남아 거실을 페인트칠 할 것이다 (조건)<br />
                            If you go fishing, will you take your camera? : 만약 낚시 하러 간다면 카메라 가지고 갈 거니? <br />
                    </li>
                    <li>
                      depend on : ~에 의지하다,  It should be : 그것은 ~으로의존하다, 좌우되다<br />
                    </li>
                    <li>
                      될 수 있다, 될 가능성이 있다
                    </li>
                    <li>
                      I guess that’s one advantage of being a bachelor : 그것이 독신이 될 하나의 이점이라고 생각한다
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
          speech:'What are you doing this weekend, Kevin?'
        },
        {
          name:'B:',
          speech:'It depends on the weather. If it’s a nice day, I’ll go fishing at Bear Lake.'
        },
        {
          name:'A:',
          speech:'What if it rains?'
        },
        {
          name:'B:',
          speech:'If it rains, I’ll stay home and paint the living room.'
        },
        {
          name:'A:',
          speech:'I’ll bet it was Jessica’s idea to paint the living room. Is she going to help you?'
        },
        {
          name:'B:',
          speech:'She’ll help me if I ask her. But I’m hoping the weather will be good so I can go to Bear Lake.'
        },
        {
          name:'A:',
          speech:'I hear it’s a beautiful place. If you go fishing, will you take your camera?'
        },
        {
          name:'B:',
          speech:'Sure. But I won’t take any pictures unless I catch some really big fish.'
        },
        {
          name:'A:',
          speech:'How’s the fishing now?'
        },
        {
          name:'B:',
          speech:'It should be excellent. Do you want to come, Peter?'
        },
        {
          name:'A:',
          speech:'Sure, I’m always free on the weekends.'
        },
        {
          name:'B:',
          speech:'Hmm. I guess that’s one advantage of being a bachelor.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'Kevin, 이번 주말에 뭐 할 거예요?'
        },
        {
          name:'B:',
          speech:'날씨에 따라 달라요. 날씨가 좋으면 Bear Lake로 낚시하러 갈 거예요.'
        },
        {
          name:'A:',
          speech:'비가 오면 어떡해요?'
        },
        {
          name:'B:',
          speech:'비가 오면 집에 있으면서 거실에 페인트칠을 할 거예요.'
        },
        {
          name:'A:',
          speech:'거실에 페인트칠을 하자는 게 Jessica의 생각이었을 거예요. 그녀가 당신을 도와줄 건가요?'
        },
        {
          name:'B:',
          speech:'내가 물어보면 그녀가 도와줄 거예요. 하지만 날씨가 좋아서 Bear Lake에 갈 수 있었으면 좋겠어요.'
        },
        {
          name:'A:',
          speech:'아름다운 곳이라고 들었어요. 낚시하러 가면 카메라를 가져가실 건가요?'
        },
        {
          name:'B:',
          speech:'물론이죠. 하지만 정말 큰 물고기를 잡지 않으면 사진을 찍지 않을 거예요.'
        },
        {
          name:'A:',
          speech:'지금 낚시는 어때요?'
        },
        {
          name:'B:',
          speech:'훌륭할 거예요. Peter, 올래요?'
        },
        {
          name:'A:',
          speech:'그럼요, 주말에는 항상 한가해요.'
        },
        {
          name:'B:',
          speech:'흠. 그게 미혼남의 한 가지 장점인 것 같아요.'
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
