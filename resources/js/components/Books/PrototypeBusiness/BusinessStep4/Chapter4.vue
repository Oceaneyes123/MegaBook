<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/lAeLs/MAD7IylAeLs/1/s2/canva-young-man-using-smartphone-and-watching-tv-in-living-room-MAD7IylAeLs.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing what’s on TV 1 
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
                            Why do they start talking about TV programs?
                        </li>
                        <li>
                            Which programs did Naomi watch last night?
                        </li>
                        <li>
                            Which two types of program do they talk about?
                        </li>
                    </ol>

                    <p>
                        Free response:<br />
                        Talk about television programs.<br />
                        What sort of TV programs are popular in your country?<br />
                        What types of programs do they like most?
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
                                                Did you watch that quiz show last night?<br />
                                                Do you have… in your country? It’s a reality TV show.<br />
                                                Have you ever seen that programme about buying property abroad?<br />
                                                I watched an interesting documentary about China last night.
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
            speech:'So, is your hotel OK? Did you sleep well?'
            },
            {
            name:'Naomi:',
            speech:'Yes, fine thanks. I watched TV for a while, then had an early night. I watched a bit of that… quiz show… Who Wants To Be A Millionaire? – the French version.'
            },
            {
            name:'Valerie:',
            speech:'Ah, really?'
            },
            {
            name:'Naomi:',
            speech:'It’s exactly the same as in the UK. The studio, the music…'
            },
            {
            name:'Valerie:',
            speech:'Yes, I think a lot of those kinds of shows are the same.'
            },
            {
            name:'Naomi:',
            speech:'Do you have The Weakest Link? It’s a quiz show, and the presenter’s really horrible at the contests.'
            },
            {
            name:'Valerie:',
            speech:'Oh, yes, Yes, it’s the same in France. I’ve seen the English version, as well, on satellite TV.'
            },
            {
            name:'Naomi:',
            speech:'And do you have programs like Big Brother? You know, with people living in a house, and there are cameras filming all the time.'
            },
            {
            name:'Valerie:',
            speech:'Yes, we had a similar thing a few years ago. Do you have that program, um… in France it’s called Star Academy… er, with people who want to be pop stars, and, er, people vote, um…'
            },
            {
            name:'Naomi:',
            speech:'Yeah. It’s called Fame Academy in England. There’ve been so many things like that on television in the last few years. Reality TV.'
            },
            {
            name:'Valerie:',
            speech:'Reality TV. Yeah. It’s been the same in France. At home, I have satellite TV, and I get English programs…'
            },
            ],

            translations:[
            {
            name:'발레리:',
            speech:'그래, 너희 호텔은 괜찮아? 잘 잤니?'
            },
            {
            name:'나오미:',
            speech:'그래, 고마워. 나는 잠시 TV를 보다가 일찍 잤어. 나는 그 퀴즈쇼를 조금 봤어. 백만장자가 되고 싶은 사람? – 프랑스어 버전.'
            },
            {
            name:'발레리:',
            speech:'아, 정말?'
            },
            {
            name:'나오미:',
            speech:'영국과 똑같아. 스튜디오, 음악...'
            },
            {
            name:'발레리:',
            speech:'응, 그런 방송들은 많이 똑같은 것 같아.'
            },
            {
            name:'나오미:',
            speech:'가장 ‘약한 고리’를 아니? 퀴즈쇼인데, 발표자가 콘테스트에서 정말 끔찍해.'
            },
            {
            name:'발레리:',
            speech:'아, 그래. 프랑스도 마찬가지야. 나는 위성 TV에서 영어 버전도 봤어.'
            },
            {
            name:'나오미:',
            speech:'그리고 너희 빅 브라더 같은 프로그램 있어? 알다시피, 사람들이 살고 있고, 카메라들이 항상 촬영하고 있어.'
            },
            {
            name:'발레리:',
            speech:'응, 몇 년 전에 비슷한 게 있었어. 프랑스에는 ’스타 아카데미’라는 프로그램이 있니? 팝스타가 되고 싶은 사람들이 있고, 음, 사람들이 투표하는...'
            },
            {
            name:'나오미:',
            speech:'응. 그것은 영국의 명예 아카데미라고 불린다. 지난 몇 년 동안 텔레비전에서 그런 일이 정말 많이 있었어. 리얼리티 TV.'
            },
            {
            name:'발레리:',
            speech:'리얼리티 TV. 응, 프랑스도 그랬어. 집에는 위성 TV가 있고 영어 프로그램도 있는데…'
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
