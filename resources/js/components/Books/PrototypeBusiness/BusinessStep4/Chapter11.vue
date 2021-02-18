<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://image.freepik.com/free-photo/elegant-director_1098-13540.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Making decisions 1 
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
                <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Translation</h3>
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
                        Underline the correct words so that the sentences are true.
                    </p>


                    <ol style="margin: 12px;">
                        <li>
                            In Germany, you should/shouldn’t be very direct.
                        </li>
                        <li>
                            In the UK, you have to/don’t have to agree all the time.
                        </li>
                        <li>
                            In Japan, you should/shouldn’t criticize people directly.
                        </li>
                        <li>
                            In Japanese companies, they often have to/don’t have to make decisions in groups.
                        </li>
                    </ol>

                    <p>
                        Read the comments about decision making. Which do you agree and disagree with? Say why.
                    </p>

                    <ol style="margin: 12px;">
                        <li>
                            'I think it's best to tell people what you really think of their suggestions, and to be direct. '
                        </li>
                        <li>
                            'If you don't agree with someone's idea, it's important not to criticise their suggestion.'
                        </li>
                        <li>
                            'In companies, it's best to make group decisions. It's important that all the team agress.'
                        </li>
                        <li>
                            'In the end, one person has to make a decision, even if the others in the team don't agree.'
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
                                                Should, have to<br />
                                                I think we <b>should</b> develop this product.<br />
                                                In my opinion, we <b>shouldn’t</b> make a decision yet.<br />
                                                We <b>have to</b> make a decision soon.<br />
                                                We <b>don’t have to</b> decide now.
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
                name:'Interviewer:',
                speech:'People often say that some nationalities are more polite than others. Do you think that’s true? And do you think you have to be more or less polite when you work with people from different cultures?'
                },
                {
                name:'Sandra:',
                speech:'You don’t have to be more or less polite. I think it’s more a question of how direct people are. You should always be polite. It’s just that, in some cultures, it’s OK to be direct, and in other, um… it’s not. For example, in Germany, people ask direct questions and… they like direct answers.'
                },
                {
                name:'Interviewer:',
                speech:'But in the UK, generally, people are less direct, aren’t they?'
                },
                {
                name:'Sandra:',
                speech:'Well, they’re not afraid to say they disagree or… or to criticize suggestions. You don’t have to say you agree all the time. But… you know, people say things like, ‘I’m not sure I agree’, or… ‘Maybe it would be better to do it another way’. I’ve always found, in different cultures, the best way to disagree or… or criticize ideas is to make it clear you’re criticizing the suggestion – you shouldn’t criticize the person.'
                },
                {
                name:'Interviewer:',
                speech:'In Japan, it’s very important not to criticize people, isn’t it?'
                },
                {
                name:'Sandra:',
                speech:'Yes, You should never criticize anyone directly. It’s… for the Japanese, it’s very impolite. That’s why, often, in companies in Japan, people have to make decisions in groups. Everyone has to agree.'
                },
                {
                name:'Interviewer:',
                speech:'So what’s your general advice? Do you think people should change the way they communicate in different cultures or… or should you just be yourself?'
                },
                {
                name:'Sandra:',
                speech:'I think you should always be yourself, um… but… I think, to be successful, you really need to change how you say things.'
                },
                ],

            translations:[
                {
                name:'인터뷰어:',
                speech:'사람들은 종종 어떤 국적은 다른 국적에 비해 더 공손하다고 말합니다. 그게 사실이라고 생각하나요? 그리고 다른 문화권의 사람들과 함께 일할 때 어느 정도 예의를 갖춰야 한다고 생각하나요?'
                },
                {
                name:'산드라:',
                speech:'좀 더 예의를 차릴 필요는 없어요. 사람들이 얼마나 직접적이냐 하는 것이 더 문제라고 생각합니디. 항상 예의 바르게 행동해야 한다. 단지, 어떤 문화권에서는 직접적이어도 괜찮고, 다른 문화권에서는 그렇지 않다는 것입니다. 예를 들어, 독일에서 사람들은 직접적인 질문을 하고… 그들은 직접적인 대답을 좋아합니다.'
                },
                {
                name:'인터뷰어:',
                speech:'하지만 영국에서는 일반적으로 사람들이 덜 직접적이잖아요, 그렇죠?'
                },
                {
                name:'산드라:',
                speech:'글쎄, 그들은 동의하지 않는다고 말하는 것, 또는 제안을 비판하는 것을 두려워하지 않아요. 항상 동의한다고 말할 필요는 없어요. 하지만, 사람들은 ’동의할 수 있을지 모르겠다’나 ’다른 방법으로 하는 게 더 나을지도 모르겠다’와 같은 말을 합니다. 저는 항상, 다른 문화권에서, 의견을 달리하거나 비평하는 가장 좋은 방법은 그 제안을 비판한다는 것을 분명히 하는 것이라는 것을 발견했습니다. 그 사람을 비판해서는 안됩니다.'
                },
                {
                name:'인터뷰어:',
                speech:'일본에서는 사람을 비판하지 않는 것이 매우 중요해요, 그렇지 않은가요?'
                },
                {
                name:'산드라:',
                speech:'그렇습니다. 당신은 절대로 누군가를 직접적으로 비난해서는 안 돼요. 그건 일본인에게 매우 무례한 행동입니다. 그렇기 때문에 일본의 기업에서는 사람들이 단체로 결정을 내려야 하는 경우가 많아요. 모두가 동의해야 합니다.'
                },
                {
                name:'인터뷰어:',
                speech:'그럼 일반적인 조언은 뭔가요? 당신은 사람들이 서로 다른 문화에서 의사소통하는 방식을 바꿔야 한다고 생각하는나요? 아니면 그냥 자신이 되어야 한다고 생각하나요?'
                },
                {
                name:'산드라:',
                speech:'전  항상 그 자신이 되어야 한다고 생각합니다. 음… 하지만… 제 생각에, 성공하기 위해서는, 말하는 방식을 바꿀 필요가 있습니다.'
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
