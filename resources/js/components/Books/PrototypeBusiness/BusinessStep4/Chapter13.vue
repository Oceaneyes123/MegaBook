<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/KYQsU/MADzI_KYQsU/1/s2/canva-woman-in-black-and-white-striped-long-sleeve-shirt-wearing-black-sunglasses-MADzI_KYQsU.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Dealing with problems 
                    </h1>
                </v-layout>
            </v-img>

            <div style=" border-color: #1A6DD9; border-style: solid; border-width: 2px;">
            </div>
            <h3 class="border white--text">Today's topic</h3>
            <div style="padding : 16px;">

                <p>
                    Rachel having a conversation during her trip.<br />
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
                        레이첼은 여행 중에 대화를 나누고 있다.<br />
                        </p>
                        <br />

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
                        Are these sentences true(T) or false(F)?
                    </p>


                    <ol style="margin: 12px;">
                        <li>
                            The next train is at 9.30 ( &emsp; )
                        </li>
                        <li>
                            Rachel’s ticket is OK for the next train. ( &emsp; )
                        </li>
                        <li>
                            She could book a seat on the next time. ( &emsp; )
                        </li>
                        <li>
                            She could go first class if she paid more. ( &emsp; )
                        </li>
                        <li>
                            She changes her ticket. ( &emsp; )
                        </li>
                        <li>
                            The next train is running on time. ( &emsp; )
                        </li>
                    </ol>

                    <p>
                        Free response:<br />
                        Talk about travel problems you’ve had, for example:<br />
                        Long delays and cancelled departures<br />
                        Missing important trains or flights<br />
                        Problems with tickets and reservations<br />
                        Traffic jams
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
                                                I’ve missed my connection. Can I catch the next train?<br />
                                                Is this ticket valid on the next train?<br />
                                                WIf I cancel the ticket, will I get a refund?<br />
                                                If I change the reservation, will I have to pay a supplement?<br />
                                                Are there any seats in first class? Can I upgrade?<br />
                                                Is the train running on time?<br />
                                                The flight’s delayed.
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
            name:'Assistant:',
            speech:'Hello.'
            },
            {
            name:'Rachel:',
            speech:'Hello. I’ve just missed my connection to London. I was booked on the nine thirty. I just want to check if my ticket is valid for the next train… at half past ten.'
            },
            {
            name:'Assistant:',
            speech:'Um… ah yes, you’re OK. Obviously, you won’t have a seat reservation.'
            },
            {
            name:'Rachel:',
            speech:'No. Is it too late to make one?'
            },
            {
            name:'Assistant:',
            speech:'Mmm, I’m afraid so.'
            },
            {
            name:'Rachel:',
            speech:'Will it be busy?'
            },
            {
            name:'Assistant:',
            speech:'It’s usually quite busy, yeah. You’ll probably get a seat in first class, if you want to change your ticket.'
            },
            {
            name:'Rachel:',
            speech:'Would I have to cancel this ticket? Would I get a refund, or…?'
            },
            {
            name:'Assistant:',
            speech:'You can just upgrade it. You just pay a supplement. I can check how much it would cost.'
            },
            {
            name:'Rachel:',
            speech:'Um… oh, no, it’s OK. I don’t think my company would pay for my expensive first class!'
            },
            {
            name:'Assistant:',
            speech:'Ah.'
            },
            {
            name:'Rachel:',
            speech:'OK, thanks. Oh… is the ten thirty on time, by the way?'
            },
            {
            name:'Assistant:',
            speech:'Um… It’s running four minutes late.'
            },
            {
            name:'Rachel:',
            speech:'OK, thanks.'
            },
            ],

            translations:[
            {
            name:'보조자:',
            speech:'안녕하세요.'
            },
            {
            name:'레이첼:',
            speech:'안녕하세요. 저는 방금 런던 운행편을 놓쳤습니다. 저는 9시 30분에 예약되었어요. 10시 30분에 제 표가 다음 열차에 유효한지 확인하려고 합니다.'
            },
            {
            name:'보조자:',
            speech:'음… 네. 분명히, 당신은 좌석을 없을거예요.'
            },
            {
            name:'레이첼:',
            speech:'안 돼요. 하나 만들기엔 너무 늦었나요?'
            },
            {
            name:'보조자:',
            speech:'음, 유감이지만요.'
            },
            {
            name:'레이첼:',
            speech:'Will it be busy?'
            },
            {
            name:'보조자:',
            speech:'보통은 꽤 붐벼요. 만약 표를 바꾸기를 원하시면 일등석을 예약하실 수 있습니다.'
            },
            {
            name:'레이첼:',
            speech:'제가 이 티켓을 취소해야 할까요? 환불해야할까요, 아니면…?'
            },
            {
            name:'보조자:',
            speech:'업그레이드만 하면 됩니다. 단지 보충금을 지불하면 됩니다. 비용이 얼마나 들지는 제가 확인해보겠습니다.'
            },
            {
            name:'레이첼:',
            speech:'음, 오, 아니, 괜찮아요. 우리 회사가 일등석의 비싼 값을 지불하지 않을 것 같아요!'
            },
            {
            name:'보조자:',
            speech:'아.'
            },
            {
            name:'레이첼:',
            speech:'고마워요. 아… 10시 30분 정각에 도착하나요?'
            },
            {
            name:'보조자:',
            speech:'음… 4분 늦어요.'
            },
            {
            name:'레이첼:',
            speech:'고마워요..'
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
