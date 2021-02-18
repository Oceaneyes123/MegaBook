<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://image.freepik.com/free-photo/portrait-interesting-reddish-man-mixing-coffee_158595-3761.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Describing a business concept 2 
                    </h1>
                </v-layout>
            </v-img>

            <div style=" border-color: #1A6DD9; border-style: solid; border-width: 2px;">
            </div>
            <h3 class="border white--text">Today's topic</h3>
            <div style="padding : 16px;">


         <p>
             Amy Venn is talking to a junior colleague about product placement.<br />
          </p>
          <br />
              
          <table style = "border-collapse: collapse;">
              
            <tr v-for="dialog in dialogs" :key="dialog">
              <td class = "uppertable" >{{dialog.name}}</td>
              <td class = "lowertable" >{{dialog.speech}}</td>
            </tr>
                
          </table>


        <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #1A6DD9; border-style: solid; border-width: 2px;">
        </div>
          <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Translation</h3>
            <div style="padding : 16px;">
              <p>
                에이미 벤은 후배와 제품 배치에 대해 이야기하고 있다.<br />
              </p>
              <br />
              
              <table style = "border-collapse: collapse;">
                
                <tr v-for="translation in translations" :key="translation">
                  <td class = "uppertable" >{{translation.name}}</td>
                  <td class = "lowertable" >{{translation.speech}}</td>
                </tr>
                
              </table>
            </div>


            <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#1A6DD9; border-style: solid; border-width: 2px;">
                   </div>
                   <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#1A6DD9;">Exercise</h3>
                   <div style="padding : 16px;">


                    <p>
                        Answer the questions.
                    </p>


                    <ol style="margin: 12px;">
                        <li>
                            Do product placements always show the company logo?
                        </li>
                        <li>
                            What product placement are very expensive?
                        </li>
                        <li>
                            What did the first product placements advertise?
                        </li>
                        <li>
                            Which company had a product placement in the film Forrest Gump?
                        </li>
                    </ol>

                    <p>
                        Free response:<br />
                        Do you think product placement can be more effective than advertising? Say way.<br />
                        In your opinion, what’s the difference between good and bad product placement?
                    </p>

                </div>

                <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #1A6DD9; border-style: solid; border-width: 2px;">
                </div>
                <h3 class="border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Self Study</h3>
                <div style="padding : 16px;">


                    <p>
                        Notes
                    </p>

                    <p>

                        <v-container grid-list-md text-xs-left>
                            <v-layout row wrap>


                                <v-flex xs12>
                                    <v-card light color="#2E97F2">
                                        <v-card-text class="px-10">
                                            <p>
                                                Useful language<br />
                                                In return for a payment, the product is shown in the film.<br />
                                                In big films, the logos on products are seen by millions of viewers.<br />
                                                Product placement was used for the first time in the 1960s.
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

    data() {

        return {

            dialogs:[
            {
            name:'Colleague:',
            speech:'So, the products are seen in films and TV programs. They’re just… seen on a table or…'
            },
            {
            name:'Amy:',
            speech:'That’s right. Or in our case, with clothes, they’re worn by an actor, um…'
            },
            {
            name:'Colleague:',
            speech:'And you see the logo.'
            },
            {
            name:'Amy:',
            speech:'Sometimes, yeah. It depends. You can’t always… control what happens. Often, products are given to the film company for free. So you know an actor is going to… to wear your jacket, for example, but… you don’t know if you’ll actually see the logo.'
            },
            {
            name:'Colleague:',
            speech:'So you can’t say to the film company, we want to… see this part of the jacket, or…'
            },
            {
            name:'Amy:',
            speech:'Well, you can, but then, usually, you have to pay. Sometimes, the film company is paid by the advertiser. And then you have more control. I mean… sometimes, the name of a product is said by an actor. But that’s… in a film – you’re talking big money for that sort of thing.'
            },
            {
            name:'Colleague:',
            speech:'Yeah, I bet… And when did companies start doing this? I guess it’s done more now than in the past.'
            },
            {
            name:'Amy:',
            speech:'I think the first placements were used in films in the 1960s, for cigarettes. But the big business really started in the 80s. I think the best placement, though, was, um… did you see Forrest Gump? The Apple placement was done very well in that.'
            },
            {
            name:'Colleague:',
            speech:'For Apple computers?'
            },
            {
            name:'Amy:',
            speech:'Yeah. There’s a scene where Forrest Gump gets a letter from Apple…'
            },
            ],

            translations:[
            {
            name:'동료:',
            speech:'그래서, 그 제품들은 영화와 TV 프로그램에서 보여져요. 그것들은 그냥 테이블에서 보여지거나...'
            },
            {
            name:'에이미:',
            speech:'맞아요. 아니면 저희의 경우, 옷이 있으면 배우가 입어요, 음…'
            },
            {
            name:'동료:',
            speech:'그리고 로고가 보이시죠.'
            },
            {
            name:'에이미:',
            speech:'가끔, 그래요. 사정에 따라 다르겠죠. 무슨 일이 일어나는지 항상 통제할 수는 없어요. 종종 영화사에 제품이 공짜로 주어져요. 예를 들어, 어떤 배우가 재킷을 입을지는 알겠지만 실제로 로고가 보일지는 알 수 없어요.'
            },
            {
            name:'동료:',
            speech:'그래서 영화사에 말할 수 없고, 자켓의 부분을 보고 싶어요.'
            },
            {
            name:'에이미:',
            speech:'음, 할 수 있지만, 보통은, 돈을 내야 해요. 때때로, 그 영화사는 광고주가 지불해요. 그리고  더 많은 통제력을 가지게 될거예요. 내 말은, 때때로, 제품의 이름은 배우에 의해 말해져요. 하지만 영화에서는 그런 것에 대해 큰 돈을 쓰는군요.'
            },
            {
            name:'동료:',
            speech:'그래요, 장담하는데… 그리고 기업들은 언제부터 이런 일을 시작했을까요? 과거보다 지금 더 많이 한 것 같아요.'
            },
            {
            name:'에이미:',
            speech:'나는 첫 번째 배치는 1960년대에 영화에, 담배에 사용되었다고 생각해요. 하지만 그 큰 사업은 정말 80년대에 시작되었어요. 제 생각엔, 포레스트 검프 봤어요? 애플 사의 배치는 그 점에서 매우 훌륭했어요.'
            },
            {
            name:'동료:',
            speech:'애플 컴퓨터요?'
            },
            {
            name:'에이미:',
            speech:'네. 포레스트 검프가 애플컴퓨터로부터 편지를 받는 장면이 있어요.'
            },

            ]

        }

    },


    beforeMount() {


    },

    methods: {


    },

    watch: {

        fontSize(current, old) {

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
  border-color: transparent #1A6DD9 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background: #1A6DD9;
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
