<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="//live.staticflickr.com/1474/25125213021_ab28e5f8a5_k.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgba(140, 103, 90, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing aims
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color:#402B24; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border white--text" >Today's topic</h3>
  <div style = "padding : 16px;">

    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table> 

    

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #402B24; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #402B24;">Translation</h3>
    <div style="padding : 16px;">

      <table style = "border-collapse: collapse;">

        <tr v-for="translation in translations" :key="translation">
          <td class = "uppertable" >{{translation.name}}</td>
          <td class = "lowertable" >{{translation.speech}}</td>
        </tr>

      </table>
   </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Exercise</h3>
      <div style="padding : 16px;">

        <p>
          Match the pairs to make sentences from the conversation.
        </p>

        <ol style="margin: 12px;">
          <li>
            If a flight costs under $50,000,
          </li>
          <li>
            If tickets cost over $500,000,
          </li>
          <li>
            If it's too short,
          </li>
          <li>
            If the first company is successful,
          </li>
        </ol>

        <ol style="margin: 12px;" type="a">
          <li>
            very few people will buy them.
          </li>
          <li>
            a lot of others will follow.
          </li>
          <li>
            I think there'll be a lot of demand.
          </li>
          <li>
            then people won't be happy.
          </li>
        </ol>

        <p>
           Free response:<br />
           Discuss these opinions about space tourism. Do you agree with any of them? Say why.
        </p>

        <ol style="margin: 12px;">
          <li>
            ‘Perhaps one day there’ll be tourism in space, but certainly not in the next ten years’
          </li>
          <li>
            ‘I think space tourism will be a big industry, and it’ll probably start in three or four years’
          </li>
          <li>
            'Maybe tourists will go into space in ten or twenty years, but only very, very rich tourists!'
          </li>
        </ol>

      </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Self Study</h3>
      <div style="padding : 16px;">


          <p>
            Notes
          </p>

        <p>

          <v-container grid-list-md text-xs-left>
            <v-layout row wrap>


              <v-flex xs12>
                <v-card light color="#F2CBBD">
                  <v-card-text class="px-10">
                <p>
                  First conditional<br />
                  <b>If</b> the project <b>is</b> uccessful, they<b>’ll</b> make a lot of money.<br />
                  There<b>’ll be</b> a lot of demand, <b>if</b> the price <b>is</b> reasonable.
                </p>
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
          name:'Interviewer:',
          speech:'Do you think we’ll see a space tourism industry in the next… five years? Is that realistic?'
        },
        {
          name:'Caroline:',
          speech:'I think so, yeah. I’m not sure how big it’ll be. It all depends how much it costs. You know, if a flight costs… under fifty thousand dollars, I think there’ll be a lot of demand. If tickets cost over five hundred thousand dollars, very few people will buy them. Obviously, it’ll be expensive. The question is, how expensive?'
        },
        {
          name:'Interviewer:',
          speech:'Some people say two hundred thousand dollars is a realistic price.'
        },
        {
          name:'Caroline:',
          speech:'Mmm… Well, that’s probably about right for a short-term objective. In the long term, I think the cost will need to be less than that. Probably less than half that.'
        },
        {
          name:'Interviewer:',
          speech:'What do you think space tourists will want? What sort of experience?'
        },
        {
          name:'Caroline:',
          speech:'Um… I think they’ll want… I think it has to be a real space trip. If it’s too short, then people won’t be happy. I don’t think it needs to last for hours, but a couple of minutes won’t be enough. It has to be worth the money.'
        },
        {
          name:'Interviewer:',
          speech:'What do you think it will take to really make space tourism take off?'
        },
        {
          name:'Caroline:',
          speech:'If somebody shows that it’s possible, for a reasonable price, I think that’ll be the start. If the first company is successful, a lot of others will follow. And, obviously, the top priority is safety. That’s the big challenge-to show that it’s safe.'
        },
        ],

        translations:[
        {
          name:'인터뷰어:',
          speech:'앞으로 5년 안에 우주 관광 산업이 나올까요? 그게 현실적인가요?'
        },
        {
          name:'캐롤라인:',
          speech:'전 그렇게 생각합니다. 얼마나 클지 모르겠지만 모든 것은 비용이 얼마냐에 달려 있습니다. 비행기 한 대가 5만 달러 이하라면 많은 돈이 들 것 같습니다. 수요의 티켓 가격이 50만 달러 이상이면 극소수의 사람들이 그것을 살 것입니다. 분명히, 그것은 비쌀 것입니다. 문제는, 얼마나 비싼가입니다.'
        },
        {
          name:'인터뷰어:',
          speech:'어떤 사람들은 20만 달러가 현실적인 가격이라고 말한다.'
        },
        {
          name:'캐롤라인:',
          speech:'음… 글쎄, 단기 목표로는 아마 거의 맞을 것입니다. 장기적으로 보면 저는 비용이 그것보다 적게 들 필요가 있을 것이라고 생각합니다. 아마 절반도 안 될 겁니다.'
        },
        {
          name:'인터뷰어:',
          speech:'우주 여행객들이 원하는 것이 무엇이라고 생각하는나요? 어떤 종류의 경험일까요?'
        },
        {
          name:'캐롤라인:',
          speech:'음… 제가 생각하기에 그들이 원하는 것은… 그것이 진짜 우주 여행이 되어야 한다고 생각합니다. 너무 짧다면 사람들은 행복하지 않을 것 입니다. 몇 시간 동안 지속할 필요는 없다고 생각하지만 몇 분이면 충분치 않을 겁니다. 그것은 그 돈의 가치가 있어야 합니다.'
        },
        {
          name:'인터뷰어:',
          speech:'우주 관광이 정말로 성공하려면 무엇이 필요할 것이라고 생각하나요?'
        },
        {
          name:'캐롤라인:',
          speech:'만약 누군가가 합리적인 가격으로 그것이 가능하다는 것을 보여준다면, 그게 시작일 것 같습니다. 첫 번째 회사가 성공한다면 다른 회사들도 많이 따라올 것입니다. 그리고, 분명히, 가장 중요한 것은 안전입니다. 그것이 안전하다는 것을 보여주는 큰 도전입니다.'
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
  border-color: transparent#402B24 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background:#402B24;
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
