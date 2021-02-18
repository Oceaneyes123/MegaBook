<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/MADGxqQurGs/5/screen_2x/canva-woman-in-black-suit-jacket-facing-man-in-blue-denim-dress-shirt-same-standing-MADGxqQurGs.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Passing on information 2 
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
                            What does Victoria say about the Darley Hotel?
                        </li>
                        <li>
                            What does she think about the hotel’s quote?
                        </li>

                        <li>
                            What’s George going to do tomorrow?
                        </li>
                        <li>
                            What’s Victoria going to do now?
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
                                                Useful language<br />
                                                She promised to finish the report this week.<br />
                                                He agreed to increase the budget by 10%.<br />
                                                We’ve decided not to start work yet.<br />
                                                He said he was happy to attend and was keen to give a talk.<br />
                                                He doesn’t like flying, so he was reluctant to go by plane.
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
                speech:'So I’ve looked at the three quotes, from all three hotels. And, obviously, we visited all three as well. Um… and I think the best place is the Darley.'
            },
            {
                name:'George:',
                speech:'Yeah. I agree. The trouble is, it’s the most expensive.'
            },
            {
                name:'Victoria:',
                speech:'Yeah. Their price is, what, ten percent higher than the other two.'
            },
            {
                name:'George:',
                speech:'Hmm. It is their first offer, though. I haven’t negotiated with them yet.'
            },
            {
                name:'Victoria:',
                speech:'No. Could you try to get a better price from them?'
            },
            {
                name:'George:',
                speech:'I can try, yeah. I’ll call the manager in the morning. Um… what’s her name… Heidi Wells.'
            },
            {
                name:'Victoria:',
                speech:'Tell her you’ve spoken to your boss, and, er… tell her I said they can have the contract if they can give us a ten percent discount.'
            },
            {
                name:'George:',
                speech:'And why don’t I show her the offers from the other hotels? I can go and see her, and take the quotes with me. That’s probably better than phoning.'
            },
            {
                name:'Victoria:',
                speech:'Yeah, OK.'
            },
            {
                name:'George:',
                speech:'And what if she says they can’t give us ten percent, but they can give… I don’t know, five percent?'
            },
            {
                name:'Victoria:',
                speech:'Well, do your best to get ten percent. If she offers you… five percent, or whatever, then… tell her you’ll have to speak to me again. Tell her you can accept ten percent immediately, but, if not, you’ll have to get back to me.'
            },
            {
                name:'George:',
                speech:'OK, fine. I’ll phone her now and see if I can arrange a meeting tomorrow.'
            },
            {
                name:'Victoria:',
                speech:'Right. I’ll give John Gates a call and give him an update – tell him what our strategy is!'
            },
            {
                name:'George:',
                speech:'So I’ll give you a call, um… after I’ve met Heidi Wells, tomorrow.'
            },
            {
                name:'Victoria:',
                speech:'Right, OK. Well good luck!'
            },
            {
                name:'George:',
                speech:'Thanks. Bye.'
            },
            ],

            translations:[
            {
                name:'빅토리아:',
                speech:'그래서 저는 세 개의 호텔 모두로부터 세 개의 인용구들을 살펴보았어요. 그리고, 분명히, 우리는 세 사람 모두를 방문했어요. 음... 그리고 내 생각에 최고의 장소는 달리입니다.'
            },
            {
                name:'조지:',
                speech:'네. 나도 동의해요. 문제는 그게 가장 비싸다는 거예요.'
            },
            {
                name:'빅토리아:',
                speech:'네, 가격이 다른 두 개보다 10% 더 비싸거든요.'
            },
            {
                name:'조지:',
                speech:'흠. 하지만 그것은 그들의 첫 번째 제안입니다. 나는 아직 그들과 협상하지 않았어요.'
            },
            {
                name:'빅토리아:',
                speech:'아니. 좀 더 싸게 해 주실 수 있어요?'
            },
            {
                name:'조지:',
                speech:'해볼 수 있어요, 네. 아침에 매니저에게 전화할게요. 음… 그녀의 이름은… 하이디 웰스예요.'
            },
            {
                name:'빅토리아:',
                speech:'상사와 얘기해 보았다고 전해주세요. 그리고, 어... 10% 할인해주면 계약서를 받을 수 있다고 전해주세요.'
            },
            {
                name:'조지:',
                speech:'그리고 제가 그녀에게 다른 호텔들의 제안을 보여주는 건 어떨까요?  그녀를 만나러 갈 수 있고, 인용문을 가지고 갈 수 있어요. 그게 아마 전화하는 것보다 나을 거예요.'
            },
            {
                name:'빅토리아:',
                speech:'네, 좋아요..'
            },
            {
                name:'조지:',
                speech:'그리고 만약 그녀가 우리에게 10%를 해줄 수는 없지만,  5%를 해줄 수 있다면 어떨까요?'
            },
            {
                name:'빅토리아:',
                speech:'음, 10%를 얻기 위해 최선을 다해야죠. 만약 그녀가 5퍼센트 혹은 그 무엇이든지 제안한다면, 그녀에게 다시 저와 이야기해야 한다고 말하세요. 그녀에게 즉시 10%제안을 받아들일 수 있다고 말하세요. 하지만 그렇지 않다면, 나에게 다시 연락해야 할 거예요.'
            },
            {
                name:'조지:',
                speech:'그래, 알았어요. 내가 지금 그녀에게 전화해서 내일 회의 일정을 잡을 수 있는지 알아볼게요.'
            },
            {
                name:'빅토리아:',
                speech:'그래요. 내가 존 게이츠에게 전화해서 업데이트 해줄게요. 우리 전략이 뭔지 말해줘요!'
            },
            {
                name:'조지:',
                speech:'그럼 내일 하이디 웰스를 만난 후에 전화할게요.'
            },
            {
                name:'빅토리아:',
                speech:'그래, 알았어요. 행운을 빕니다!'
            },
            {
                name:'조지:',
                speech:'고마워요. 안녕'
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


</style>
