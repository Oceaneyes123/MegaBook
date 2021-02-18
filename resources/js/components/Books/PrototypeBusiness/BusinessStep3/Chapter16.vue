<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGxyccMIo/4/screen_2x/canva-view-of-tourist-resort--MADGxyccMIo.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Forecasting 
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
          Are these sentences true(T) or false(F)<br />
          Caroline thinks
        </p>

        <ol style="margin: 12px;">
          <li>
            the resort will possibly be successful in the long term. (&emsp;)
          </li>
          <li>
            the number of visitors will probably be low in the first few months. (&emsp;)
          </li>
          <li>
            it definitely won’t help to predict the success of other resorts. (&emsp;)
          </li>
          <li>
            the resort will certainly be popular with families. (&emsp;)
          </li>
          <li>
            perhaps somebody will build another dome, somewhere. (&emsp;)
          </li>
          <li>
            maybe there’s a very large market for tropical domes. (&emsp;)
          </li>
        </ol>

        <p>
           Free response:<br />
           Talk about tropical domes.<br />
           Do you think the Berlin resort will be successful in the long term?<br />
           Do you think companies will build comes in other locations?
        </p>

        <p>
          Talk about a project you're planning or starting soon. Explain what you want to do, then make forecasts about the project.
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
                  Will: predictions<br />
                  I <b>think</b> the project <b>will</b> be successful.<br />
                  I <b>don’t think</b> it’ll be very successful. (it’ll = it will)<br />
                  Personally, I <b>think it’ll / it won’t</b> be a success.
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
          speech:'What do you think about the location of the resort, near Berlin?'
        },
        {
          name:'Caroline:',
          speech:'Well, the reason it’s there is, simply, because there was already a dome there. Tropical Islands Resort didn’t build the dome. They bought it, for quite a low price. A company called CargoLifter built the dome as a factory, to make big airships. But CargoLifter went out of business and had to sell the dome. So Tropical Islands bought it and… so they had very low construction costs.'
        },
        {
          name:'Interviewer:',
          speech:'So, do they think the resort’ll be successful in the long term?'
        },
        {
          name:'Caroline:',
          speech:'Possibly. I think it’ll probably be quite popular in the short term… in the first few months. I think a lot of people’ll probably come to have a look… they’ll want to see what it’s like. After that, it depends what they think of it.'
        },
        {
          name:'Interviewer:',
          speech:'Some people say this resort won’t help to make forecasts for other resorts because there was no need to build a dome. Do you agree with that?'
        },
        {
          name:'Caroline:',
          speech:'Um… no. I think it’ll help a lot. Definitely. The construction costs aren’t difficult to calculate. The difficult question is, what sort of people will visit the dome? I’m sure it’ll be popular with families with young children, for example. So, the project’ll be good for getting information about the market.'
        },
        {
          name:'Interviewer:',
          speech:'Do you think someone will build another dome like this somewhere, one day?'
        },
        {
          name:'Caroline:',
          speech:'It’s possible, yeah. Maybe there’s a huge market for them. I mean, it’s not a completely new idea. There’s already a dome like this one in Japan.'
        },
        ],


        translations:[
        {
          name:'인터뷰어:',
          speech:'베를린 근처에 있는 리조트의 위치에 대해 어떻게 생각하십니까?'
        },
        {
          name:'캐롤라인:',
          speech:'음, 그게 거기 있는 이유는, 간단히 말해서, 거기에는 이미 돔이 있었기 때문입니다. 열대섬 리조트는 돔을 짓지 않았습니다. 그들은 꽤 싼 값에 그것을 샀습니다. 카고라이프터라는 회사는 큰 비행선을 만들기 위해 돔을 공장으로 만들었습니다. 그러나 카고라이프터는 폐업하여 돔을 팔아야 했습니다. 그래서 트로피컬 아일랜드가 그것을 샀고 그래서 그들은 매우 낮은 건축비를 가지고 있었습니다.'
        },
        {
          name:'인터뷰어:',
          speech:'그렇다면, 그들은 이 리조트가 장기적으로 성공할 것이라고 생각하나요?'
        },
        {
          name:'캐롤라인:',
          speech:'아마도 내 생각에 그것은 아마도 단기간에 꽤 인기가 있을 것 같아요… 처음 몇 달 동안은. 아마 많은 사람들이 어떤 모습인지 보고 싶어할 겁니다. 그 이후에는 그들이 어떻게 생각하느냐에 따라 달라질거예요.'
        },
        {
          name:'인터뷰어:',
          speech:'어떤 사람들은 이 리조트가 돔을 지을 필요가 없었기 때문에 다른 리조트의 예측에 도움이 되지 않을 것이라고 말합니다 당신은 그것에 동의하시나요?'
        },
        {
          name:'캐롤라인:',
          speech:'음…아니요. 도움이 많이 될 것 같아요. 물론. 공사비는 계산하기 어렵지 않습니다. 어려운 질문은, 어떤 종류의 사람들이 돔을 방문할까 하는 것입니다. 어린 자녀가 있는 가족들에게 인기가 많을 겁니다. 예를 들면 그래서, 그 프로젝트는 시장에 대한 정보를 얻는 데 좋을 것입니다.'
        },
        {
          name:'인터뷰어:',
          speech:'언젠가 누군가가 이런 돔을 또 지을 거라고 생각하시나요?'
        },
        {
          name:'캐롤라인:',
          speech:'가능합니다. 어쩌면 그들에게 엄청난 시장이 있을지도 모릅니다. 내 말은, 완전히 새로운 생각은 아닙니다. 일본에는 이미 이런 돔이 있습니다.'
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
