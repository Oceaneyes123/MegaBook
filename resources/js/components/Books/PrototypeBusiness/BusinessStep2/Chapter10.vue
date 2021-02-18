<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGwITUbVY/5/screen_2x/canva-train-station-MADGwITUbVY.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgba(254, 183, 43, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Making choices
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border" >Today's topic</h3>
  <div style = "padding : 16px;">

    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table>

    
        <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
            </div>
            <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Translation</h3>
            <div style="padding : 16px;">

              <table style = "border-collapse: collapse;">

                <tr v-for="translation in translations" :key="translation">
                  <td class = "uppertable" >{{translation.name}}</td>
                  <td class = "lowertable" >{{translation.speech}}</td>
                </tr>

              </table>
          </div>
  
  
    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Exercise</h3>
    <div style="padding : 16px;">

      <p>
        Make superlatives.
      </p>

      <ol style="margin: 12px;">
        <li>
          flying/safe way to travel<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          a high-speed train/ convenient way to travel<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          what/good way/get to the airport?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
      </ol>

      <p>
        Free response:<br />
        Compare travelling by plane, train and car. What are the advantages and disadvantages?<br />
        Give your opinion for each of these situations.
      </p>
      <p>
        - a one-day business trip to another city.<br />
        - a week at a conference in another city<br />
        - a holiday abroad
      </p>

    </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Self Study</h3>
    <div style="padding : 16px;">


      <p>
        Notes
      </p>

      <p>

        <v-container grid-list-md text-xs-left>
          <v-layout row wrap>


            <v-flex xs12>
              <v-card light color="#527318">
                <v-card-text class="px-10">
                  <p>
                    Superlatives
                  </p>
                  <p>
                    Short adjectives<br />
                    <b>the</b> cheap<b>est</b><br />
                    <b>the</b> fast<b>est</b><br />
                  </p>
                  <p>
                    Long adjectives<br />
                    <b>the most</b> expensive<br />
                    <b>the least</b> convenient
                  </p>
                  <p>
                    Irrgular adjectives<br />
                    good><b>the best</b><br />
                    bad><b>the worst</b>
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
          name:'A:',
          speech:'What time do we get to Frankfurt? Quarter past?'
        },
        {
          name:'B:',
          speech:'Um... yes. Yes, we’re on time, I think. The last time I took this flight it was about an hour late.'
        },
        {
          name:'A:',
          speech:'Yeah? I don’t usually fly. I normally go to Frankfurt on the train.'
        },
        {
          name:'B:',
          speech:'From Paris?'
        },
        {
          name:'A:',
          speech:'Yeah. It takes... six and a half hours.'
        },
        {
          name:'B:',
          speech:'Hmm.'
        },
        {
          name:'A:',
          speech:'It’s not a high-speed train.'
        },
        {
          name:'B:',
          speech:'No. I drove last year, from Paris to Frankfurt. It took me... six hours, I think.'
        },
        {
          name:'A:',
          speech:'Right.'
        },
        {
          name:'B:',
          speech:'No, the fastest way is by plane. Definitely.'
        },
        {
          name:'A:',
          speech:'Oh yeah, I agree. I think the train’s the most convenient way, though. There’s more space. so you can work. You arrive right in the city center.'
        },
        {
          name:'B:',
          speech:'Oh, I’m not so sure. For me the most convenient way is the fastest way. I prefer to fly.'
        },
        {
          name:'A:',
          speech:'Well, I suppose, for me, It’s a question of cost, really. The train’s cheaper.'
        },
        {
          name:'B:',
          speech:'How much is it to Frankfurt?'
        },
        {
          name:'A:',
          speech:'From Paris? It’s about, um... a hundred and eighty euros.'
        },
        {
          name:'B:',
          speech:'Yeah. You’re right. And that’s cheaper than going by car. With fuel and running costs.'
        },
        {
          name:'A:',
          speech:'Hmm. I don’t like driving. I think it’s the worst way to travel. For longer distances.'
        },
        {
          name:'B:',
          speech:'Yes, that’s true. When I drove to Frankfurt, I arrived at about...'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'프랑크푸르트에 몇 시에 가? 15분 후?'
        },
        {
          name:'B:',
          speech:'음... 응, 제시간에 온 것 같아 내가 이 비행기를 마지막으로 탔을 때는 한 시간 정도 늦었어.'
        },
        {
          name:'A:',
          speech:'응? 나는 보통 비행기를 타지 않아. 나는 보통 기차를 타고 프랑크푸르트에 가.'
        },
        {
          name:'B:',
          speech:'파리에서?'
        },
        {
          name:'A:',
          speech:'응. 6시간 반이나 걸려.'
        },
        {
          name:'B:',
          speech:'흠.'
        },
        {
          name:'A:',
          speech:'고속 열차는 아니야.'
        },
        {
          name:'B:',
          speech:'아니. 작년에 파리에서 프랑크푸르트까지 운전했어. 내가... 6시간 정도?'
        },
        {
          name:'A:',
          speech:'그렇구나.'
        },
        {
          name:'B:',
          speech:'아니, 비행기로 가는 게 제일 빨라. 물론이지.'
        },
        {
          name:'A:',
          speech:'래, 나도 동의해. 그래도 기차가 제일 편할 것 같아. 공간이 더 넓어. 네가 일할 수 있게 말이야. 너는 바로 도심에 도착해.'
        },
        {
          name:'B:',
          speech:'오, 잘 모르겠어. 나에게 가장 편리한 방법은 가장 빠른 방법이다. 나는 나는 것을 더 좋아한다.'
        },
        {
          name:'A:',
          speech:'글쎄, 내 생각엔, 이건 정말 비용 문제인 것 같아. 기차가 더 싸다.'
        },
        {
          name:'B:',
          speech:'프랑크푸르트까지 얼마야?'
        },
        {
          name:'A:',
          speech:'파리에서? 그건, 음... 백팔십 유로'
        },
        {
          name:'B:',
          speech:'그렇구나. 네 말이 맞아. 그리고 그것은 차로 가는 것보다 싸. 연료와 운영비.'
        },
        {
          name:'A:',
          speech:'흠. 난 운전하는 거 싫어해. 운전이 여행하는 데 제일 안 좋은 방법인 것 같아. 장거리용으로.'
        },
        {
          name:'B:',
          speech:'그래, 맞아. 프랑크푸르트까지 차를 몰고 갔을 때, 나는 대략...'
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
  border-color: transparent #899857 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background: #899857;
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
