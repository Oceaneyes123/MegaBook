<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/aqj9o/MADyRPaqj9o/1/s2/canva-man-standing-in-front-of-airplane-MADyRPaqj9o.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing safety procedures
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

                    <ol style="margin: 12px;">
                        <li>
                            What’s the biggest danger on the tarmac?
                        </li>
                        <li>
                            Why is the danger in question 1 worse at airport?
                        </li>
                        <li>
                            Which the problem with ear protection?
                        </li>
                        <li>
                            What’s the problem with ear protection?
                        </li>
                        <li>
                            What other words does Dennis use for danger and dangerous?
                        </li>
                    </ol>

                    <p>
                        Free response:<br />
                        Talk about safety in your job, company or industry, or another industry you know about.<br />
                        What are the main dangers?<br />
                        What safety precautions must workers take and what procedures must they follow?
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
                                                Must<br />
                                                All pilots <b>must</b> have a license.<br />
                                                (= They have to have one.)<br />
                                                You <b>mustn’t</b> carry dangerous items on planes. (= You’re not allowed to.)
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
                name:'Dennis:',
                speech:'OK. Let’s make a list of dangers on the tarmac… and then we can make a list of safety precautions to help prevent accidents. So, first of all, what are the main hazards? Any suggestions?'
                },
                {
                name:'Woman:',
                speech:'Planes, when they’re moving.'
                },
                {
                name:'Dennis:',
                speech:'OK…. Moving planes.'
                },
                {
                name:'Man:',
                speech:'Noise from engines… from the jets. You need to wear ear protection.'
                },
                {
                name:'Dennis:',
                speech:'Uhuh, OK. Noise… protection.'
                },
                {
                name:'Woman:',
                speech:'Other vehicles, moving around.'
                },
                {
                name:'Dennis:',
                speech:'OK, good. Moving vehicles. They are the biggest hazard on the tarmac. Not planes, but vehicles: buses, trucks, cars… What precautions can you take to help avoid accidents – to prevent ground vehicles hitting people?'
                },
                {
                name:'Woman:',
                speech:'Er, everyone should wear a green jacket.'
                },
                {
                name:'Dennis:',
                speech:'OK. High visibility clothing. Essential. Does anyone know why moving vehicles are especially dangerous at airports?'
                },
                {
                name:'Woman:',
                speech:'Because they drive around quite fast?'
                },
                {
                name:'Dennis:',
                speech:'They often do, yeah. They’re not allowed to, though, The health and safety regulations say that every employee is responsible for the safety of others. But there’s another reason why moving vehicles are particularly hazardous at airports. Any other ideas?'
                },
                {
                name:'Man:',
                speech:'Because you can’t hear them, because of all the noise… from jets and, um…'
                },
                {
                name:'Dennis:',
                speech:'Exactly. If you’re standing near a plane with its engines running, you can’t always hear vehicles coming. Just now, someone said you need to wear ear protection. For some jobs - for example, if you have to stand in front of moving planes to guide the pilots, then, yes, you need to protect your ears. But only some people need ear protection, some of the time.'
                },
                {
                name:'Woman:',
                speech:'So how do we know if we need ear protection or not? Are there standard procedures?'
                },
                {
                name:'Dennis:',
                speech:'Yes. We’ll look at those a bit later on…'
                },
            ],

            translations:[
            {
                name:'데니스:',
                speech:'좋아요. 활주로에 위험요인 목록을 만든 다음 안전 예방조치 목록을 만들어 사고 예방에 도움을 주도록 합시다. 그렇다면, 우선, 주요 위험은 무엇인가요? 좋은 의견이라도 있으신가요?'
                },
                {
                name:'W:',
                speech:'비행기가 움직일 때요.'
                },
                {
                name:'데니스:',
                speech:'그래요… 움직이는 비행기.'
                },
                {
                name:'M:',
                speech:'엔진에서 나는 소음... 제트기에서 나는 소음. 귀 보호대를 착용해야 합니다.'
                },
                {
                name:'데니스:',
                speech:'으응, 알았어요. 소음… 보호.'
                },
                {
                name:'W:',
                speech:'다른 차량들, 돌아다니고 있어요.'
                },
                {
                name:'데니스:',
                speech:'좋아요. 움직이는 차량. 그들은 활주로에서 가장 큰 위험요소입니다. 비행기가 아니라 차량: 버스, 트럭, 자동차… 지상 차량이 사람을 치지 않도록 하기 위해 어떤 예방 조치를 취할 수 있을까요?'
                },
                {
                name:'W:',
                speech:'음, 모든 사람들은 녹색 재킷을 입어야 해요.'
                },
                {
                name:'데니스:',
                speech:'알겠어요. 가시성이 높은 의류. 필수적. 움직이는 차량이 공항에서 특히 위험한 이유를 아는 사람있나요?'
                },
                {
                name:'W:',
                speech:'그들이 운전을 빨리 해서요?'
                },
                {
                name:'데니스:',
                speech:'그들은 종종 그래요. 하지만, 보건 안전 규정에 따르면, 모든 직원들이 다른 사람들의 안전에 책임이 있다고 합니다. 그러나 움직이는 차량이 공항에서 특히 위험한 이유는 또 있습니다. 다른 생각 있나요?'
                },
                {
                name:'M:',
                speech:'왜냐하면, 제트기에서 나오는 소음 때문에, 음...'
                },
                {
                name:'데니스:',
                speech:'바로 그거예요. 만약 당신이 엔진을 가동하고 비행기 근처에 서 있다면, 당신은 항상 차가 오는 소리를 들을 수 없습니다. 방금 귀 보호대를 착용해야 한다고 하셨어요. 예를 들어, 만약 당신이 조종사들을 안내하기 위해 움직이는 비행기 앞에 서야 한다면, 그렇습니다, 당신은 귀를 보호할 필요가 있습니다. 하지만 오직 일부 사람들만이 귀 보호가 필요한 경우도 있습니다.'
                },
                {
                name:'W:',
                speech:'그렇다면, 귀 보호가 필요한지 아닌지 어떻게 알 수 있을까요? 표준적인 절차가 있나요?'
                },
                {
                name:'데니스:',
                speech:'네. 조금 이따가 이 사진들을 봅시다.'
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
