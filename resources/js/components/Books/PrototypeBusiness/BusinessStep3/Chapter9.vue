<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGx6w_XSg/4/screen_2x/canva-building-beside-shore-MADGx6w_XSg.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Describing places 
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color:#402B24; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border white--text" >Today's topic</h3>
  <div style = "padding : 16px;">

    <p>
      Alistair Alby, from New Zealand, is on a business trip in Hawaii. He's having lunch with Caroline Carmen, a colleague. <br />
    </p>
    <br />

    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Translation</h3>
    <div style="padding : 16px;">
     


        <p>
          뉴질랜드에서 온 알리스테어 알비는 하와이로 출장 중이다. 그는 동료 캐롤라인 카르멘과 점심을 먹고 있다.<br />
          </p>
          <br />

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
 


        <ol style="margin: 12px;">
          <li>
            What does Alistair like about Hawaii?
          </li>
          <li>
            What time of year is it in New Zealand?
          </li>
          <li>
            Why does Alistair talk about Christmas dinner?
          </li>
          <li>
            What’s the name of the mountains he talks about?
          </li>
          <li>
            What does he say about travelling on the South Island?
          </li>
        </ol>

        <p>
           Free response:<br />
           Talk about a tourist destination, in your country or abroad, that you would like to visit and say why.
        </p>

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
                  Useful language :<br />
                  What’s it like there?<br />
                  It’s beautiful. The beaches are really nice.<br />
                  It’s in the mountains, but it’s not too far from the sea.<br />
                  What’s the weather like in summer?<br />
                  What’s the best time of year to visit?
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
          name:'Caroline:',
          speech:'So, what do you think of Hawaii?'
        },
        {
          name:'Alistair:',
          speech:'Fantastic. The beaches are amazing. We’ve got some good surfing beaches in New Zealand, but here it’s… well, the weather’s a lot warmer, that’s the first difference… at this time of year, anyway.'
        },
        {
          name:'Caroline:',
          speech:'Of course, it’s winter in New Zealand, isn’t it?'
        },
        {
          name:'Alistair:',
          speech:'Yeah. It’ll soon be spring, though.'
        },
        {
          name:'Caroline:',
          speech:'I’d like to go, actually… maybe not this year, but… possibly next year.'
        },
        {
          name:'Alistair:',
          speech:'To New Zealand?'
        },
        {
          name:'Caroline:',
          speech:'Yeah. What’s the best time of year to visit?'
        },
        {
          name:'Alistair:',
          speech:'Early summer’s nice. Late December, early January.'
        },
        {
          name:'Caroline:',
          speech:'And what’s the weather like?'
        },
        {
          name:'Alistair:',
          speech:'Pretty hot, usually. You can have Christmas dinner on the beach, no problem! But there’s a lot more to do than just sit on a beach, obviously.'
        },
        {
          name:'Caroline:',
          speech:'Oh, sure. So, what are the best places to see?'
        },
        {
          name:'Alistair:',
          speech:'The nicest part of the country’s South Island, in my opinion, anyway. You go to the mountains there, the Southern Alps, and it’s… oh, it’s beautiful.'
        },
        {
          name:'Caroline:',
          speech:'So, do you need a car to travel round?'
        },
        {
          name:'Alistair:',
          speech:'Yeah. Or you can rent a camper van. That’s what a lot of people do. There are hundreds of campsites, where you can…, you know, park and…'
        },
        {
          name:'Caroline:',
          speech:'Yeah. Yeah.'
        },
        {
          name:'Alistair:',
          speech:'I know that area pretty well, so…'
        },
        {
          name:'Caroline:',
          speech:'Can you recommend some campsites?'
        },
        {
          name:'Alistair:',
          speech:'Yeah, I can give you some good addresses. There’s one campsite, next to a lake…'
        },
        ],

        translations:[
        {
          name:'캐롤라인:',
          speech:'그래, 너는 하와이에 대해 어떻게 생각하니?'
        },
        {
          name:'알리스테어:',
          speech:'환상적이야. 해변은 정말 멋져. 뉴질랜드에는 좋은 서핑 해변이 몇 군데 있지만, 여기엔… 날씨가 훨씬 따뜻해, 그게 첫 번째 차이야… 어쨌든 이맘때면 말이야.'
        },
        {
          name:'캐롤라인:',
          speech:'물론 뉴질랜드가 겨울이지?'
        },
        {
          name:'알리스테어:',
          speech:'그래, 하지만 곧 봄이 될 거야.'
        },
        {
          name:'캐롤라인:',
          speech:'사실 올해는 아닐지 몰라도 내년에는 가고 싶어.'
        },
        {
          name:'알리스테어:',
          speech:'뉴질랜드로?'
        },
        {
          name:'캐롤라인:',
          speech:'응. 일 년 중 언제 방문하기에 가장 좋을까?'
        },
        {
          name:'알리스테어:',
          speech:'초여름은 좋아. 12월 하순, 1월 초순.'
        },
        {
          name:'캐롤라인:',
          speech:'날씨는 어때?'
        },
        {
          name:'알리스테어:',
          speech:'보통은 꽤 덥지. 크리스마스 저녁은 해변에서 먹을 수 있어, 문제 없어! 하지만 분명히 해변에 그냥 앉아 있는 것 말고도 할 일이 훨씬 더 많다.'
        },
        {
          name:'캐롤라인:',
          speech:'아, 물론이지. 그렇다면, 가장 보기 좋은 곳은 어디일까?'
        },
        {
          name:'알리스테어:',
          speech:'내 생각에는, 어쨌든, 이 나라의 가장 좋은 곳은 남섬이야. 산으로 가면, 알프스 남쪽에 있는 산으로 가면, 오, 아름다워.'
        },
        {
          name:'캐롤라인:',
          speech:'그래서, 너는 차가 필요하니, 여행 때문에?'
        },
        {
          name:'알리스테어:',
          speech:'아니면 캠핑카를 빌릴 수도 있어. 많은 사람들이 그렇게 해. 수백 개의 야영지가 있는데, 그곳에는 주차할 수 있고…'
        },
        {
          name:'캐롤라인:',
          speech:'그래.'
        },
        {
          name:'알리스테어:',
          speech:'나는 그 지역을 잘 알고 있어서…'
        },
        {
          name:'캐롤라인:',
          speech:'야영지를 좀 추천해 줄래?'
        },
        {
          name:'알리스테어:',
          speech:'응, 좋은 주소 몇 개 줄 수 있어. 캠핑장이 하나 있는데, 호수 옆에…'
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
