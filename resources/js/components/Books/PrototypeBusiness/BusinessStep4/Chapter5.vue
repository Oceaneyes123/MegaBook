<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="//live.staticflickr.com/33/103466903_ca2a2980ac_h.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing what’s on TV 2
                    </h1>
                </v-layout>
            </v-img>

            <div style=" border-color: #1A6DD9; border-style: solid; border-width: 2px;">
            </div>
            <h3 class="border white--text">Today's topic</h3>
            <div style="padding : 16px;">

                <table style = "border-collapse: collapse;">

                    <tr v-for="dialog in dialogs" :key="dialog">
                      <td class = "uppertable" >{{dialog.name}}</td>
                      <td class = "lowertable" >{{dialog.speech}}</td>
                    </tr>
              
                  </table>


                <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #1A6DD9; border-style: solid; border-width: 2px;">
                </div>
                <h3 class="border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Translation</h3>
                <div style="padding : 16px;">
                
                      <table style = "border-collapse: collapse;">
                
                        <tr v-for="translation in translations" :key="translation">
                          <td class = "uppertable" >{{translation.name}}</td>
                          <td class = "lowertable" >{{translation.speech}}</td>
                        </tr>
                
                      </table>
                   </div>

                   
                    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #1A6DD9; border-style: solid; border-width: 2px;">
                    </div>
                    <h3 class="border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Exercise</h3>
                    <div style="padding : 16px;">


                    <p>
                        Answer the questions.
                    </p>


                    <ol style="margin: 12px;">
                        <li>
                            What sort of channel is BBC Prime?
                        </li>
                        <li>
                            What programs does Valerie find hard to understand?
                        </li>
                        <li>
                            Why does Naomi laugh?
                        </li>
                        <li>
                            What are two ways of showing films in another language?
                        </li>
                    </ol>

                    <p>
                        Free response:<br />
                        In your opinion, what are the worst programs on TV? Why don’t you like them?<br />
                        Do you think watching TV is good or bad for children? Why?
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
                                                useful language<br />
                                                What channel is it on?<br />
                                                Have you got satellite or cable TV?<br />
                                                Do you get the …. Channel?<br />
                                                Does the film have subtitles or is it dubbed?
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
            name:'Valerie:',
            speech:'At home, I have satellite TV, and I get English programs on BBC Prime. They show things like quiz shows, documentaries, comedy programs. I find comedies quite difficult to understand.'
            },
            {
            name:'Naomi:',
            speech:'Yeah, I bet.'
            },
            {
            name:'Valerie:',
            speech:'There’s a talk show, as well, where they interview famous people, I think the presenter’s very well known in Britain. His name’s, um… oh…'
            },
            {
            name:'Naomi:',
            speech:'Michael Parkinson?'
            },
            {
            name:'Valerie:',
            speech:'Yes! They also show some good children’s programs. My little boy watches Teletubbies.'
            },
            {
            name:'Naomi:',
            speech:'Oh yeah.'
            },
            {
            name:'Valerie:',
            speech:'There’s another thing I sometimes watch. What’s the name for the type of programs…. It’s about, not real people, they’re actors, but about… just everyday life in a street or, um…'
            },
            {
            name:'Naomi:',
            speech:'A soap opera. Or a soap.'
            },
            {
            name:'Valerie:',
            speech:'That’s it! There’s a soap about the people who live in a… a square in London. I… I can’t remember…'
            },
            {
            name:'Naomi:',
            speech:'Not EastEnders?'
            },
            {
            name:'Valerie:',
            speech:'EastEnders. That’s it. What’s so funny?'
            },
            {
            name:'Naomi:',
            speech:'Valerie, I can’t believe you watch EastEnders… in Paris!'
            },
            {
            name:'Valerie:',
            speech:'Actually, I’d like to watch more films in English. On French TV, when they show American films, the voices are in French. How do you say that? They’re…'
            },
            {
            name:'Naomi:',
            speech:'Dubbed.'
            },
            {
            name:'Valerie:',
            speech:'Dubbed?'
            },
            {
            name:'Naomi:',
            speech:'Yeah.'
            },
            {
            name:'Valerie:',
            speech:'They’re nearly always dubbed in French. On some channels, they show the original film with er… you know, text at the bottom of the screen with… with the translation.'
            },
            {
            name:'Naomi:',
            speech:'With subtitles?'
            },
            {
            name:'Valerie:',
            speech:'Subtitles, yeah. But I don’t like that because you read but you don’t really listen to…'
            },
            ],

            translations:[
            {
            name:'발레리:',
            speech:'집에는 위성 TV가 있고, BBC 프라임에서 영어 프로그램을 들어. 그들은 퀴즈 쇼, 다큐멘터리, 코미디 프로그램 같은 것들을 보여줘. 나는 희극이 꽤 이해하기 어렵다고 생각해.'
            },
            {
            name:'나오미:',
            speech:'그래, 완전.'
            },
            {
            name:'발레리:',
            speech:'토크쇼도 있고, 유명한 사람들을 인터뷰하는 토크쇼도 있는데, 나는 발표자가 영국에서 아주 잘 알려져 있다고 생각해. 그의 이름은, 음… 오…'
            },
            {
            name:'나오미:',
            speech:'마이클 파킨슨?'
            },
            {
            name:'발레리:',
            speech:'맞아! 그들은 또한 몇몇 좋은 어린이 프로그램들을 보여줘. 내 어린 아들은 텔레토비를 봐.'
            },
            {
            name:'나오미:',
            speech:'아 그래.'
            },
            {
            name:'발레리:',
            speech:'가끔 보는 게 또 있어. 프로그램 종류에 대한 이름이..  진짜 사람이 아니라 배우라는 건데, 그냥 길거리에서 일상생활을 하는 거야.'
            },
            {
            name:'나오미:',
            speech:'연속극. 아니면 드라마.'
            },
            {
            name:'발레리:',
            speech:'바로 그거야! 런던의 광장에 사는 사람들에 대한 연속극이 있어. 기억이 안 나는데…'
            },
            {
            name:'나오미:',
            speech:'이스트엔더스 말고?'
            },
            {
            name:'발레리:',
            speech:'이스트엔더스. 바로 그거야. 뭐가 그렇게 웃겨?'
            },
            {
            name:'나오미:',
            speech:'발레리, 파리에서 이스트엔더스를 보다니 믿을 수가 없어!'
            },
            {
            name:'발레리:',
            speech:'사실, 나는 영어로 된 더 많은 영화를 보고 싶어. 프랑스 TV에서, 그들이 미국 영화를 상영할 때, 그 목소리는 프랑스어로 나와. 어떻게 그렇게 말할까? 그들은…'
            },
            {
            name:'나오미:',
            speech:'더빙.'
            },
            {
            name:'발레리:',
            speech:'더빙?'
            },
            {
            name:'나오미:',
            speech:'응.'
            },
            {
            name:'발레리:',
            speech:'그것들은 거의 항상 프랑스어로 더빙돼. 어떤 채널에서는 원작을 번역과 함께 화면 하단에 텍스트와 함께 보여줘.'
            },
            {
            name:'나오미:',
            speech:'자막으로?'
            },
            {
            name:'발레리:',
            speech:'응, 자막. 하지만 당신이 읽지만 잘 듣지 않기 때문에 나는 그것을 좋아하지 않는다.'
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
