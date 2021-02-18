<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/IayKo/MAD35zIayKo/1/s2/canva-woman-in-white-crew-neck-t-shirt-using-silver-macbook-MAD35zIayKo.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Passing on information 1 
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
                            What information does Victoria need?
                        </li>
                        <li>
                            Does George have the information?
                        </li>

                        <li>
                            Where’s George going next?
                        </li>
                        <li>
                            What’s he doing this afternoon?
                        </li>
                    </ol>

                    <p>
                        How often do you talk about discussions you had with other people? Think about:<br />
                        - taking and receiving telephone messages<br />
                        - telling colleagues what was discussed in meetings they didn't attend<br />
                        - giving feedback about discussions with customers or suppliers
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
                                                Report speech<br />
                                                I’<b>m</b>very busy. > He said he <b>was</b> very busy.<br />
                                                I <b>have</b> a copy. > He said he <b>had</b> a copy.<br />
                                                I <b>can</b> email it. > He said he <b>could</b> email it.<br />
                                                I’<b>ll</b> send it. > He said he <b>would</b> send it.
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
                name:'George:',
                speech:'Hello.'
            },
            {
                name:'Victoria:',
                speech:'Hello George, it’s Victoria. How are you?'
            },
            {
                name:'George:',
                speech:'Not too bad.'
            },
            {
                name:'Victoria:',
                speech:'I’m just calling about the quotes, from the three hotels, for the conference. Have you got copies of all of them?'
            },
            {
                name:'George:',
                speech:'Um… yes. Yeah, they’re here on my, er, desk… somewhere.'
            },
            {
                name:'Victoria:',
                speech:'Could you email them to me?'
            },
            {
                name:'George:',
                speech:'Um… I can fax them. I’ve only got hard copies – I haven’t got the files in the computer, so, um…'
            },
            {
                name:'Victoria:',
                speech:'OK, fine.'
            },
            {
                name:'George:',
                speech:'I’ve got to go to a meeting in about a quarter of an hour, so… I’ll send them now.'
            },
            {
                name:'Victoria:',
                speech:'Yeah, OK. There’s no rush. This afternoon’s fine, if, um…'
            },
            {
                name:'George:',
                speech:'No, no, it’s no problem. I’ll send them now.'
            },
            {
                name:'Victoria:',
                speech:'OK, great. Then maybe we can discuss them later today?'
            },
            {
                name:'George:',
                speech:'Sure. I’ll be in the office all afternoon.'
            },
            {
                name:'Victoria:',
                speech:'OK. I’ll call you later this afternoon, then.'
            },
            {
                name:'George:',
                speech:'OK.'
            },
            ],

            translations:[
            {
                name:'조지:',
                speech:'여보세요.'
            },
            {
                name:'빅토리아:',
                speech:'안녕하세요. 조지, 빅토리아예요. 잘 지내시죠?'
            },
            {
                name:'조지:',
                speech:'그렇게 나쁘진 않아요.'
            },
            {
                name:'빅토리아:',
                speech:'세 호텔의 견적서 때문에 전화한 겁니다. 회의에 쓰려고요. 전부 복사해 놓으셨어요?'
            },
            {
                name:'조지:',
                speech:'음… 그래요, 여기 내 책상 위에 있어요.'
            },
            {
                name:'빅토리아:',
                speech:'그것들을 나에게 이메일로 보내 주시겠습니까?'
            },
            {
                name:'조지:',
                speech:'음… 팩스로 보낼 수 있어요. 인쇄본 밖에 없어요. 컴퓨터에 파일이 없어서, 음…'
            },
            {
                name:'빅토리아:',
                speech:'알겠습니다.'
            },
            {
                name:'조지:',
                speech:'약 15분 후에 회의에 가야 하니까, 지금 보내줄게요.'
            },
            {
                name:'빅토리아:',
                speech:'그래, 알았어요. 서두를 필요 없어요. 오늘 오후는 괜찮아요, 음…'
            },
            {
                name:'조지:',
                speech:'아니, 아니, 문제 없어요. 지금 보낼게요.'
            },
            {
                name:'빅토리아:',
                speech:'그래, 좋아요. 그럼 우리는 오늘 나중에 토론할 수 있을까요?'
            },
            {
                name:'조지:',
                speech:'물론이죠. 오후 내내 사무실에 있을 겁니다.'
            },
            {
                name:'빅토리아:',
                speech:'알았어요. 그럼 이따 오후에 전화할게요.'
            },
            {
                name:'조지:',
                speech:'알았어요.'
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
