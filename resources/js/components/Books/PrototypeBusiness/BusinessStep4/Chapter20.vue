<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/MADGyZF51Eo/4/screen_2x/canva-person-wears-multicolored-blazer-MADGyZF51Eo.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Welcoming visitors
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
              
                    <br />
                    <p>
                    4<br />
                    </p>
                    <br />
              
                      
                    <table style = "border-collapse: collapse;">
              
                      <tr v-for="fourthdialog in fourthdialogs" :key="fourthdialog">
                        <td class = "uppertable" >{{fourthdialog.name}}</td>
                        <td class = "lowertable" >{{fourthdialog.speech}}</td>
                      </tr>
                
                    </table>
              
              
              <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #1A6DD9; border-style: solid; border-width: 2px;">
              </div>
              <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Exercise</h3>
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
              
                <br />
                <p>
                4<br />
                </p>
                <br />
              
              
                <table style = "border-collapse: collapse;">
              
              
                  <tr v-for="fourthtranslation in fourthtranslations" :key="fourthtranslation">
                    <td class = "uppertable" >{{fourthranslation.name}}</td>
                    <td class = "lowertable" >{{fourthtranslation.speech}}</td>
                  </tr>
              
                </table>
              </div>

                <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #1A6DD9; border-style: solid; border-width: 2px;">
                </div>
                <h3 class="border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Exercise</h3>
                <div style="padding : 16px;">

                    <p>
                        Find sentences from the conversations to match 1-9.
                    </p>

                    <ol style="margin: 12px;">
                        <li>
                            Apologising for not arriving on time.   <u>&emsp; &emsp; &emsp;</u>Sorry I'm late.<u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>
                        <li>
                            Inviting someone to go through a door before you.   <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>

                        <li>
                            Saying someone will come to meet you soon.   <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>
                        <li>
                            Inviting someone to sit down.   <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>

                        <li>
                            Asking if it's OK to open the window.   <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>
                        <li>
                            Suggesting a break.   <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>
                        <li>
                            Offering to take someone's coat.   <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>
                        <li>
                            Giving something to someone.   <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>
                        <li>
                            Offering someone a drink.   <u>&emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;</u>
                        </li>
                    </ol>

                    <p>
                        - Write a list of things people do and say when they welcome visitors to their company.<br />
                        - Can you give examples of how people from different countries welcome visitors?
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
                                                Have a seat. Mr. Johnson will be with you in a moment.<br />
                                                Sorry I’m late.<br />
                                                That’s OK.<br />
                                                My office is through here. After you.<br />
                                                Shall I take your coat?<br />
                                                Thanks. Here you are.<br />
                                                Do you mind if I open the window?<br />
                                                No, not at all.<br />
                                                Shall we take a break?<br />
                                                Yes, good idea.<br />
                                                Can I get you anything to drink?<br />
                                                No, I’m find thanks.
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
                name:'Amelia:',
                speech:'Hi, Tom.'
                },
                {
                name:'Tom:',
                speech:'Hi, Amelia. How are you?'
                },
                {
                name:'Amelia:',
                speech:'Very well, thanks. How are you?'
                },
                {
                name:'Tom:',
                speech:'Fine, thank you. Sorry I’m late.'
                },
                {
                name:'Amelia:',
                speech:'That’s OK'
                },
                {
                name:'Tom:',
                speech:'My train was delayed.'
                },
                {
                name:'Amelia:',
                speech:'Oh, the trains here are never on time...'
                },
            ],

            seconddialogs:[
            {
                name:'Tom:',
                speech:'Hello.'
                },
                {
                name:'Receptionist:',
                speech:'Hello.'
                },
                {
                name:'Tom:',
                speech:'I’ve come for a meeting with Amelia Donovan. My name’s Tom Watts. I’m afraid I’m a little bit late.'
                },
                {
                name:'Receptionist:',
                speech:'I’ll give her a call... Amelia, Tom Watts is in reception... OK. She’ll be with you in a moment. If you’md like to have a seat.'
                },
                {
                name:'Tom:',
                speech:'Thanks.'
                },
            ],

            thirddialogs:[
            {
                name:'Tom:',
                speech:'We’ve made good progress there.'
                },
                {
                name:'Amelia:',
                speech:'Yeah. We’re about halfway through the agenda.'
                },
                {
                name:'Tom:',
                speech:'It’s quite hot in here. Do you mind if I open the window?'
                },
                {
                name:'Amelia:',
                speech:'No, not at all. Shall we take a break?'
                },
                {
                name:'Tom:',
                speech:'Yes, good idea.'
                },
                {
                name:'Amelia:',
                speech:'We can go out and get some fresh air, if you like. We can walk across to the cafeteria and get a coffee over there...'
                },
            ],

            fourthdialogs:[
            {
                name:'Amelia:',
                speech:'OK. This is my office. After you.'
                },
                {
                name:'Tom:',
                speech:'Thank you.'
                },
                {
                name:'Amelia:',
                speech:'Shall I take your coat?'
                },
                {
                name:'Tom:',
                speech:'Yes, thank you... Here you are.'
                },
                {
                name:'Amelia:',
                speech:'Thanks. Can I get you anything to drink? Coffee? Tea?'
                },
                {
                name:'Tom:',
                speech:'No, I’m fine thanks.'
                },
                {
                name:'Amelia:',
                speech:'We can start straight away, if you like. I’ll give you a copy of...'
                },

            ],

            firsttranslations:[
            {
                name:'아멜리아:',
                speech:'안녕, 톰.'
                },
                {
                name:'톰:',
                speech:'안녕, 아멜리아. 안녕?'
                },
                {
                name:'아멜리아:',
                speech:'그래, 고마워. 안녕?'
                },
                {
                name:'톰:',
                speech:'좋아, 고마워. 늦어서 미안해.'
                },
                {
                name:'아멜리아:',
                speech:'괜찮아.'
                },
                {
                name:'톰:',
                speech:'내 기차가 연착됐어.'
                },
                {
                name:'아멜리아:',
                speech:'아, 여기 기차는 절대 제시간에 오지 않아...'
                },
            ],

            secondtranslations:[
            {
                name:'톰:',
                speech:'안녕하세요.'
                },
                {
                name:'접수 담당자:',
                speech:'안녕하세요'
                },
                {
                name:'톰:',
                speech:'아멜리아 도노반과의 미팅을 하러 왔어요. 제 이름은 톰 와츠입니다. 조금 늦은 것 같아요.'
                },
                {
                name:'접수 담당자:',
                speech:'제가 그녀에게 전화할게요... 아멜리아, 톰 와츠가 접수 중입니다... 알겠습니다. 곧 오실 겁니다. 앉고 싶으시면요.'
                },
                {
                name:'톰:',
                speech:'감사합니다.'
                },
            ],

            thirdtranslations:[
            {
                name:'톰:',
                speech:'우리는 그곳에서 좋은 진전을 이루었습니다.'
                },
                {
                name:'아멜리아:',
                speech:'그래요. 우리는 의제를 절반 정도 진행 중입니다.'
                },
                {
                name:'톰:',
                speech:'여기는 꽤 덥네요. 창문을 열어도 될까요?'
                },
                {
                name:'아멜리아:',
                speech:'그럼요. 잠시 쉬었다 갈까요?'
                },
                {
                name:'톰:',
                speech:'네, 좋은 생각이에요.'
                },
                {
                name:'아멜리아:',
                speech:'괜찮으시다면 나가서 바람 좀 쐴 수 있어요. 건너편 카페테리아로 걸어가서 커피라도 한잔 해요.'
                },

            ],

            fourthtranslations:[
            {
                name:'아멜리아:',
                speech:'알았어요. 여기는 제 사무실입니다. 먼저 가세요.'
                },
                {
                name:'톰:',
                speech:'감사합니다.'
                },
                {
                name:'아멜리아:',
                speech:'코트를 가져갈까요?'
                },
                {
                name:'톰:',
                speech:'네, 고마워요... 여기 있습니다.'
                },
                {
                name:'아멜리아:',
                speech:'고마워요. 뭐 좀 마실래요? 커피요? 차요?'
                },
                {
                name:'톰:',
                speech:'아뇨, 저는 괜찮아요.'
                },
                {
                name:'아멜리아:',
                speech:'원하신다면 바로 시작할 수 있어요. 제가 당신에게 사본을 하나 드리겠습니다.'
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
