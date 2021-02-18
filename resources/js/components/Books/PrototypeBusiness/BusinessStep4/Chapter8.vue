<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/GzPw8/MAD1uDGzPw8/1/s2/canva-person-in-white-long-sleeve-shirt-holding-pen-MAD1uDGzPw8.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing strategies
                    </h1>
                </v-layout>
            </v-img>

            <div style=" border-color: #1A6DD9; border-style: solid; border-width: 2px;">
            </div>
            <h3 class="border white--text">Today's topic</h3>
            <div style="padding : 16px;">

                <p>
                    Tony Ellston is talking to Jane Rye, an investment banker. She’s advising him on business strategy.<br />
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
                <h3 class="border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #1A6DD9;">Translation</h3>
                    <div style="padding : 16px;">
                
                      <p>
                        토니 엘스턴은 투자 은행가인 제인 례와 이야기를 나누고 있다. 그녀는 그에게 사업 전략을 조언하고 있다.<br />
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
                        Are these sentences true(T) or false(F)?
                    </p>


                    <ol style="margin: 12px;">
                        <li>
                            Tony's business has had problems recently. ( &emsp; )
                        </li>
                        <li>
                            He's planning to build a new factory. ( &emsp; )
                        </li>
                        <li>
                            He needs to hire some employees. ( &emsp; )
                        </li>
                        <li>
                            He wants to borrow money from the bank. ( &emsp; )
                        </li>
                        <li>
                            Jane asks Tony about his long-term future. ( &emsp; )
                        </li>
                    </ol>

                    <p>
                        Make sentences about yourself using each of these adverbs.<br />
                        - carefully, hard, well, quickly, easily<br />
                        I always check figures carefully.
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
                                                Adverbs of manner<br />
                                                It’s not a <b>quick</b> job. We can’t do it <b>quickly.</b><br />
                                                Our growth has been <b>gradual.</b><br />
                                                We’re grown <b>gradually.</b><br />
                                                He’s a <b>hard</b> worker. He works <b>hard.</b> (irregular)
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
                name:'Tony:',
                speech:'The business has done well over the last three years. And I think now’s the right time to expand – to open a new office, hire some good people… hire a manager to help me, and … you know, become a bigger organization. So I need to raise finance, and to do that, I’d like to try and find some people who want to buy shares in the company.'
                },
                {
                name:'Jane:',
                speech:'Right. So you’re not planning to borrow the money?'
                },
                {
                name:'Tony:',
                speech:'No. And to expand quickly. I need more than just money. I need your advice on how to manage the expansion.'
                },
                {
                name:'Jane:',
                speech:'OK. Well, you’re certainly right to recruit a manager for the new office. I’m sure you know what it’s like to work hard, seven days a week… Obviously, you’re an entrepreneur, you set up the company. But as the organization grows, each year, your job changes gradually. If you open a new office, obviously that’s a big change, so your job needs to change significantly.'
                },
                {
                name:'Tony:',
                speech:'Sure.'
                },
                {
                name:'Jane:',
                speech:'Have you thought about your future with the company?'
                },
                {
                name:'Tony:',
                speech:'… You mean, do I want to sell the whole business?'
                },
                {
                name:'Jane:',
                speech:'No, that’s not what I mean. It’s just that, if I find you some investors, they’ll want some management control. It won’t really be your business any more. You understand what I’m getting…'
                },
                {
                name:'Tony:',
                speech:'Sure, sure.'
                },
                {
                name:'Jane:',
                speech:'It’s not a decision you can make easily. But you need to think about your future carefully…'
                },

            ],

            translations:[
            {
                name:'토니:',
                speech:'그 사업은 지난 3년 동안 잘 돼 왔어요. 그리고 지금이 새로운 사무실을 열고, 좋은 사람들을 고용하고, 나를 도울 매니저를 고용하고, 더 큰 조직이 될 때라고 생각합니다. 그래서 나는 재정을 조달해야 하고, 그러기 위해서는 회사 주식을 사려는 사람들을 찾아보고 싶어요.'
                },
                {
                name:'제인:',
                speech:'맞아요. 그럼 돈을 빌릴 생각은 없으신 겁니까?'
                },
                {
                name:'토니:',
                speech:'네. 그리고 빠르게 확장하기 위해서. 나는 단지 돈 이상의 것이 필요합니다. 확장 관리 방법에 대한 당신의 조언이 필요해요.'
                },
                {
                name:'제인:',
                speech:'알았어요. 글쎄, 새 사무실에 매니저를 채용하는 것은 확실히 맞는 말이에요. 일주일에 7일은 열심히 일하는 게 어떤 건지 잘 알고 있을 거예요… 분명히, 당신은 기업가이고, 회사를 차린 거예요. 하지만 조직이 성장함에 따라, 매년 당신의 일은 점차 변화해요. 사무실을 새로 열면 분명히 큰 변화가 생기기 때문에 일이 크게 바뀌어야 해요.'
                },
                {
                name:'토니:',
                speech:'물론이죠.'
                },
                {
                name:'제인:',
                speech:'회사에서의 미래에 대해 생각해 봤어요?'
                },
                {
                name:'토니:',
                speech:'그 말은, 사업 전체를 팔고 싶단 건가요?'
                },
                {
                name:'제인:',
                speech:'아니, 내 말은 그게 아니예요. 투자자들을 찾으면 경영권을 원할 거예요. 더 이상 당신이 상관할 일이 아니죠. 무슨 말인지 아시잖아요'
                },
                {
                name:'토니:',
                speech:'물론이죠..'
                },
                {
                name:'제인:',
                speech:'그건 당신이 쉽게 결정할 수 있는 결정이 아닙니다. 하지만 당신은 미래에 대해 신중하게 생각해 볼 필요가 있어요.'
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
