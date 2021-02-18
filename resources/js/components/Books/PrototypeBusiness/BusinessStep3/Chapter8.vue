<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADQ5P5nIq4/1/screen/canva-architects-at-work-MADQ5P5nIq4.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Discussing strengths and weaknesses 
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
          Are these sentences true(T) or false(F)?
        </p>

        <ol style="margin: 12px;">
          <li>
            A coffee machine is an optional extra. (&emsp;)
          </li>
          <li>
            It’s important to have lots of light. (&emsp;)
          </li>
          <li>
            Open plan offices are more expensive. (&emsp;)
          </li>
        </ol>

        <p>
           Free response:<br />
           What do you think of your company's offices? What do you like about them? What don't you like?
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
                  Superlatives<br />
                  (+) small : This is the smallest office.<br />
                  (+) expensive : This is the most expensive.<br />
                  (-) expensive : That’s the least expensive.<br />
                  (+) good/bad : I think this is the best and that’s the worst.
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
          speech:'So, when you design an office, where do you start?'
        },
        {
          name:'Steve:',
          speech:'Well, the first question is, how much space do you need? And that’s one of the most difficult questions, sometimes because for most people, it’s difficult to say, oh I need…fifteen square meters, for example. So you have to look at what people need to do in the office, look at what equipment they need – you know, most people need a phone, a computer, um…a desk! Then there’s shared equipment,… you normally have a room with a photocopier, printers… a fax machine, possibly.'
        },
        {
          name:'Interviewer:',
          speech:'A coffee machine.'
        },
        {
          name:'Steve:',
          speech:'Oh, a coffee machine is essential! It’s important where you put it. Do you put it in a corridor, with no windows… or next to the toilets… you know, so people have short coffee breaks. Or do you have a nice coffee area, with seats… a bit consideration. Light’s extremely important.'
        },
        {
          name:'Interviewer:',
          speech:'So you want big windows, if possible.'
        },
        {
          name:'Steve:',
          speech:'Yeah, you usually want a lot of light.'
        },
        {
          name:'Interviewer:',
          speech:'What do you think of open-plan offices? Do you like that sort of design?'
        },
        {
          name:'Steve:',
          speech:'Well, an open-plan office isn’t really a design, is it? It’s just a big room, um…But we’re talking about the requirements for offices, and the most important question is money. You know, cost is always the biggest problem. At the end of the day, walls cost money. If they’re not an essential requirement, then why have them? With anything that costs money, clients always ask, is it really necessary? Offices are expensive, even if you only have what’s in the regulations – what’s compulsory. So, if something’s an optional extra…'
        },
        ],

        translations:[
        {
          name:'인터뷰어:',
          speech:'그렇다면, 사무실을 설계할 때, 어디서부터 시작하나요?'
        },
        {
          name:'스티브:',
          speech:'음, 첫 번째 질문은, 얼마나 많은 공간이 필요한가 하는 것입니다. 그게 가장 어려운 질문 중 하나입니다. 때때로 대부분의 사람들에게, 예를 들어, 15평방미터가 필요하다고 말하기 어렵기 때문입니다. 그러니까 사무실에서 사람들이 해야 할 일을 보고, 어떤 장비가 필요한지 봐야 합니다. 대부분의 사람들은 전화기, 컴퓨터, 책상이 필요해요! 그리고 공유 장비도 있고, 보통 복사기, 프린터, 팩스기가 있는 방이 있을 겁니다.'
        },
        {
          name:'인터뷰어:',
          speech:'커피머신.'
        },
        {
          name:'스티브:',
          speech:'오, 커피 머신은 필수적이죠! 어디에 두느냐가 중요합니다. 창문도 없는 복도에 두거나 화장실 옆에 두거나 그래서 사람들이 짧은 커피 휴식 시간을 가질 수 있습니다. 아니면 좋은 커피 공간이 있으신지요, 좌석이 좀... 여유가 있으신지요. 빛은 아주 중요해요.'
        },
        {
          name:'인터뷰어:',
          speech:'가능하면 큰 창문을 원하시는 거지요.'
        },
        {
          name:'스티브:',
          speech:'그래요, 보통 많은 빛을 원해요.'
        },
        {
          name:'인터뷰어:',
          speech:'오픈 플랜(건물내부가 벽으로 나뉘지 않은) 사무실들에 대해 어떻게 생각하십니까? 그런 디자인이 마음에 드십니까?'
        },
        {
          name:'스티브:',
          speech:'음, 오픈 플랜 사무실은 사실 디자인이 아니잖아요, 그렇죠? 그냥 큰 방인데, 음…그런데 사무실 요건을 얘기하는데 가장 중요한 문제는 돈입니다. 알다시피, 비용은 항상 가장 큰 문제입니다. 결국 벽은 돈이 듭니다. 만약 그것들이 필수적인 요구사항이 아니라면, 왜 그것들을 가지고 있을까요? 돈이 드는 것은 무엇이든지 간에, 고객은 항상 그것이 정말 필요한가?라고 묻습니다. 사무실은 비록 당신이 규정안에 있는 것, 즉 의무적인 것만을 가지고 있더라도 비쌉니다. 그래서, 만약 어떤 것이 선택적인 추가 사항이라면…'
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
