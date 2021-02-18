<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://image.freepik.com/free-photo/front-desk-lady-offering-tourist-fill-out-documents_1262-16110.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Using tourist facilities 
                    </h1>
                </v-layout>
            </v-img>

            <div style=" border-color: #1A6DD9; border-style: solid; border-width: 2px;">
            </div>
            <h3 class="border white--text">Today's topic</h3>
            <div style="padding : 16px;">


                    <p>
                    1<br />
                    </p>
                    <br />
              
                    <table style = "border-collapse: collapse;">
              
                      <tr v-for="firstdialog in firstdialogs" :key="firstdialog">
                        <td class = "uppertable" >{{firstdialog.name}}</td>
                        <td class = "lowertable" >{{firstdialog.speech}}</td>
                      </tr>
                
                    </table>

                    <br />
                    <p>
                    2<br />
                    </p>
                    <br />
              
                      
                    <table style = "border-collapse: collapse;">
              
                      <tr v-for="seconddialog in seconddialogs" :key="seconddialog">
                        <td class = "uppertable" >{{seconddialog.name}}</td>
                        <td class = "lowertable" >{{seconddialog.speech}}</td>
                      </tr>
                
                    </table>

                    <br />
                    <p>
                    3<br />
                    </p>
                    <br />
              
                      
                    <table style = "border-collapse: collapse;">
              
                      <tr v-for="thirddialog in thirddialogs" :key="thirddialog">
                        <td class = "uppertable" >{{thirddialog.name}}</td>
                        <td class = "lowertable" >{{thirddialog.speech}}</td>
                      </tr>
                
                    </table>

                    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #1A6DD9; border-style: solid; border-width: 2px;">
                    </div>
                    <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Translation</h3>
                    <div style="padding : 16px;">
                    
                        <p>
                        1<br />
                        </p>
                        <br />
                    
                      <table style = "border-collapse: collapse;">
                    
                    
                        <tr v-for="firsttranslation in firsttranslations" :key="firsttranslation">
                          <td class = "uppertable" >{{firsttranslation.name}}</td>
                          <td class = "lowertable" >{{firsttranslation.speech}}</td>
                        </tr>
                    
                      </table>

                      <br />
                        <p>
                        2<br />
                        </p>
                        <br />


                        <table style = "border-collapse: collapse;">


                            <tr v-for="secondtranslation in secondtranslations" :key="secondtranslation">
                            <td class = "uppertable" >{{secondtranslation.name}}</td>
                            <td class = "lowertable" >{{secondtranslation.speech}}</td>
                            </tr>

                        </table>

                        <br />
                        <p>
                        3<br />
                        </p>
                        <br />
                      
                      
                        <table style = "border-collapse: collapse;">
                      
                      
                          <tr v-for="thirdtranslation in thirdtranslations" :key="thirdtranslation">
                            <td class = "uppertable" >{{thirdtranslation.name}}</td>
                            <td class = "lowertable" >{{thirdtranslation.speech}}</td>
                          </tr>
                      
                        </table>
                    </div>

                <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #1A6DD9; border-style: solid; border-width: 2px;">
                </div>
                <h3 class="border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Exercise</h3>
                <div style="padding : 16px;">

                    <p>
                        Answer the questions<br />
                        Conversation1
                    </p>

                    <ol style="margin: 12px;">
                        <li>
                            What’s the gym called?
                        </li>
                        <li>
                            How many saunas are there on the ship?
                        </li>

                        <p style="margin-left : -35px;">
                            Conversation2
                        </p>


                        <li>
                            Why doesn’t the TV in the man’s room work?
                        </li>
                        <li>
                            How much does it cost for television?
                        </li>


                        <p style="margin-left : -35px;">
                            Conversation3
                        </p>


                        <li>
                            What does the woman want to book?
                        </li>
                        <li>
                            Why is it necessary to reserve seats?
                        </li>
                    </ol>

                    <p>
                        Free response:<br />
                        Have you ever travelled on board a ship, or been on a cruise?<br />
                        Say what you’d like and what you wouldn’t like about spending time on a ship.
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
                                                Can anyone use the gym? Is there a sauna in there?<br />
                                                I think there’s a problem with the shower in my room.<br />
                                                Do you sell international adapters for electrical sockets?<br />
                                                I’d like some information about entertainment on board.<br />
                                                Is it free?<br />
                                                There’s a small charge.
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

            firstdialogs:[
            {
            name:'Assistant:',
            speech:'Hello.'
            },
            {
            name:'Woman:',
            speech:'Hello. I’d like some information about the gym.'
            },
            {
            name:'Assistant:',
            speech:'The health and fitness club?'
            },
            {
            name:'Woman:',
            speech:'Yes. Is it open to everyone? Can anyone go in?'
            },
            {
            name:'Assistant:',
            speech:'Yes, sure.'
            },
            {
            name:'Woman:',
            speech:'And is that where the sauna is?'
            },
            {
            name:'Assistant:',
            speech:'There is a sauna in the health and fitness club, yes. There’s another on Deck C, next to the swimming pool, as well.'
            },
            {
            name:'Woman:',
            speech:'OK…. OK, thanks very much.'
            },
            ],

            seconddialogs:[
            {
            name:'Man:',
            speech:'Hi.'
            },
            {
            name:'Assistant:',
            speech:'Good morning.'
            },
            {
            name:'Man:',
            speech:'I think there’s a problem with the TV in my room. I can’t switch it on for some reason.'
            },
            {
            name:'Assistant:',
            speech:'Have you put the card in?'
            },
            {
            name:'Man:',
            speech:'The card?.... I didn’t see a card with it, um….'
            },
            {
            name:'Assistant:',
            speech:'Right. You need a card. There’s a small charge if you want TV. It’s eighteen dollars for the full ten-day cruise.'
            },
            {
            name:'Man:',
            speech:'Eighteen dollars?'
            },
            {
            name:'Assistant:',
            speech:'Yes. You just need to sign a form. Then we give you a card, and you put it on the TV. You get all the major satellite channels sir.'
            },

            ],

            thirddialogs:[
            {
            name:'Woman:',
            speech:'Excuse me, I’ve just read the poster, over there, about the show in the, um… Laguna bar tomorrow night. It says you need to book. Are there any tickets left?'
            },
            {
            name:'Assistant:',
            speech:'Yes.'
            },
            {
            name:'Woman:',
            speech:'OK. And how much are they?'
            },
            {
            name:'Assistant:',
            speech:'They’re free. It’s just it’s usually quite popular, so we prefer to issue tickets, then people aren’t disappointed if they don’t get a seat.'
            },
            {
            name:'Woman:',
            speech:'Right. OK, so can I book two seats, please?'
            },
            {
            name:'Assistant:',
            speech:'Sure, Can I take your room number.'
            },
            ],

            firsttranslations:[
            {
            name:'보조자:',
            speech:'안녕하세요.'
            },
            {
            name:'W:',
            speech:'안녕하세요. 저는 체육관에 대한 정보를 좀 알고 싶습니다.'
            },
            {
            name:'보조자:',
            speech:'헬스장이요?'
            },
            {
            name:'W:',
            speech:'네. 모든 사람들에게 열려있나요? 아무나 들어갈 수 있나요?'
            },
            {
            name:'보조자:',
            speech:'네, 물론이지요.'
            },
            {
            name:'W:',
            speech:'그리고 거기 사우나가 있나요?'
            },
            {
            name:'보조자:',
            speech:'헬스클럽에 사우나가 있어요, 네. 수영장 옆에 있는 C갑판에도 또 있습니다.'
            },
            {
            name:'W:',
            speech:'알았어요. 정말 고마워요.'
            },

            ],

            secondtranslations:[
            {
            name:'M:',
            speech:'안녕하세요.'
            },
            {
            name:'보조원 :',
            speech:'좋은 아침입니다.'
            },
            {
            name:'M:',
            speech:'제 방에 있는 TV에 문제가 있는 것 같아요. 왠지 켜지 못하겠어요.'
            },
            {
            name:'보조원 :',
            speech:'카드 넣으셨어요?'
            },
            {
            name:'M:',
            speech:'카드?.... 카드가 있는 건 못 봤는데, 음…'
            },
            {
            name:'보조원 :',
            speech:'카드가 필요해요. TV를 원하면 조금의 요금을 내야 해요. 10일 내내 유람하는 데 18달러 입니다.'
            },
            {
            name:'M:',
            speech:'18달러?'
            },
            {
            name:'보조원 :',
            speech:'네. 서류에 서명만 하면 돼요. 그러면 우리가 당신에게 카드를 주면, 당신은 그것을 TV에 넣습니다. 주요 위성 채널은 다 확보했습니다.'
            },            

            ],

            thirdtranslations:[
            {
            name:'W:',
            speech:'실례합니다만, 방금 저기 포스터를 읽었는데, 내일 밤 라구나 바에서 열리는 쇼에 대해. 예약해야 한다고 쓰여 있어서요. 남은 표가 있나요?'
            },
            {
            name:'보조자 :',
            speech:'네.'
            },
            {
            name:'W:',
            speech:'알겠습니다. 그것들은 얼마인가요?'
            },
            {
            name:'보조자 :',
            speech:'무료입니다. 그냥 보통 꽤 인기가 있어서, 우리는 표를 발행하는 것을 선호해요, 그러면 사람들은 좌석을 얻지 못해도 실망하지 않아요.'
            },
            {
            name:'W:',
            speech:'그래요, 그럼 두 자리 예약할 수 있을까요?'
            },
            {
            name:'보조자 :',
            speech:'네, 방 번호 좀 알려주시겠습니까?'
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
