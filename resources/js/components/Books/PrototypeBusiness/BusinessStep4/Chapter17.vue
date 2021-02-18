<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/k1aT4/MADyQ4k1aT4/1/s2/canva-group-of-person-sitting-indoors-MADyQ4k1aT4.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Attending meetings 
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
                            Why can’t John Gates come to the meeting?
                        </li>
                        <li>
                            What happened last week?
                        </li>
                        <li>
                            What’s the aim of this meeting?
                        </li>
                    </ol>

                    <p>
                        Talk about meetings.
                    </p>

                    <ol style="margin: 12px;">
                        <li>
                            How often do you go to meetings?
                        </li>
                        <li>
                            What sort of meetings do you attend?
                        </li>
                        <li>
                            How much time do you spend in meetings?
                        </li>
                    </ol>

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
                                                Time clauses<br />
                                                I’<b>ll call</b> you when I <b>get</b> to the station.<br />
                                                I’<b>ll phone</b> you as soon as I <b>arrive.</b><br />
                                                We <b>won’t start</b> before you <b>arrive.</b><br />
                                                We’<b>ll wait</b> until everyone <b>is</b> here.
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
                name:'Victoria:',
                speech:'OK. Shall we make a start? … er, just to say, John Gates can’t make it. He sends his apologies. He’s had to go to an urgent meeting with a customer. John’s asked me to chair the meeting… so I’m in the hot seat! OK, first, has everyone got an agenda? John told me copies were circulated on Monday.'
                },
                {
                name:'George:',
                speech:'I got the agenda, but I didn’t get a copy of the minutes from the meeting last week.'
                },
                {
                name:'Victoria:',
                speech:'The meeting last week?'
                },
                {
                name:'George:',
                speech:'John told me you all met last week, to talk about the conference. I didn’t attend. I wasn’t here last week. So I don’t know what…'
                },
                {
                name:'Victoria:',
                speech:'Oh, that. No, we didn’t hold a meeting. We didn’t take minutes or anything, it was just… some of us had a talk. during a coffee break…'
                },
                {
                name:'George:',
                speech:'Oh, OK.'
                },
                {
                name:'Victoria:',
                speech:'Don’t worry, you didn’t miss anything. So, we’ve called this meeting to talk about the sales conference next January. We need to look at the program… to plan what we’re going to do.. during the two days. So let’s look at the first item on the agenda, then: the main theme for the conference. As you know, each year we have a theme…'
                },
            ],

            translations:[
            {
                name:'빅토리아:',
                speech:'알았어. 우리 먼저 시작할까? …어, 말하자면 존 게이츠는 올 수 없습니다. 그는 사과의 말을 전했습니다 . 그는 손님과 긴급한 회의에 가야만 했습니다. 존이 나에게 회의의 의장을 맡아달라고 부탁해서 저는 난처한 입장에 처하게 되었습니다! 좋아요, 먼저 다들 안건이 있나요? 존은 나에게 월요일에 복사본이 배포되었다고 말했습니다.'
                },
                {
                name:'조지:',
                speech:'의제는 받았지만, 지난 주 회의록의 복사본은 받지 못했어요.'
                },
                {
                name:'빅토리아:',
                speech:'지난주 미팅이요?'
                },
                {
                name:'조지:',
                speech:'존이 당신들이 지난 주에 회의에 대해 이야기하려고 만났다고 저한테 말했어요. 저는 참석하지 않았습니다. 나는 지난주에 여기에 없었어요. 그래서 전 잘 모르겠습니다.'
                },
                {
                name:'빅토리아:',
                speech:'오, 그거. 아니, 우리는 회의를 열지 않았어요. 우리는 몇 분도 안 걸리고 그냥... 우리 중 몇 명이 커피를 마시면서 대화를 나눴어요.'
                },
                {
                name:'조지:',
                speech:'오, 알았어요.'
                },
                {
                name:'빅토리아:',
                speech:'걱정하지 마세요, 당신은 하나도 놓치지 않았어요. 그래서 우리는 내년 1월에 있을 영업 회의에 대해 이야기하기 위해 이 회의를 소집했습니다. 우리가 할 일을 계획하려면 프로그램을 봐야 해요. 이틀 동안. 그럼 의제의 첫 번째 항목을 살펴보도록 합시다. 회의의 주요 주제. 당신도 알다시피, 매년 우리는 테마를 가지고 있어요.'
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
