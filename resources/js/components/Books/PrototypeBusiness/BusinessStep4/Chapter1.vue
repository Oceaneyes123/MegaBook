 <template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/MADQtjo4N98/2/screen_2x/canva-extreme-paragliding-in-beautiful-paradise-MADQtjo4N98.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 class="upper-header-BS4">Discussing interesting experience
                    </h1>
                </v-layout>
            </v-img>

            <div class="line-top-BS4">
            </div>
            <h3 class="lower-header-BS4 white--text">Today's topic</h3>
            <div style="padding : 16px;">

              <table style = "border-collapse: collapse;">

                <tr v-for="dialog in dialogs" :key="dialog">
                  <td class = "uppertable" >{{dialog.name}}</td>
                  <td class = "lowertable" >{{dialog.speech}}</td>
                </tr>
          
              </table> 


                <div class = "line-BS4">
                </div>
                <h3 class = "border-BS4 white--text">Translation</h3>
                <div style="padding : 16px;">
                    

                  <table style = "border-collapse: collapse;">
    
            <tr v-for="translation in translations" :key="translation">
              <td class = "uppertable" >{{translation.name}}</td>
              <td class = "lowertable" >{{translation.speech}}</td>
            </tr>
    
          </table>
       </div>



                <div class = "line-BS4">
                </div>
                <h3 class = "border-BS4 white--text">Exercise</h3>
                <div style="padding : 16px;">

                    <p>
                        Are these sentences true(T) or false(F)?
                    </p>

                    <ol style="margin: 12px;">
                        <li>
                            Lisa did a parachute jump last year. ( &emsp; )
                        </li>
                        <li>
                            She enjoyed the experience. ( &emsp; )
                        </li>
                        <li>
                            She was frightened before she jumped. ( &emsp; )
                        </li>
                        <li>
                            After her parachute opened, she was scared. ( &emsp; )
                        </li>
                        <li>
                            She had a very hard landing. ( &emsp; )
                        </li>
                    </ol>

                    <p>
                        Free response:<br />
                        Talk about your most memorable or interesting experiences.
                    </p>

                </div>

                <div class = "line-BS4">
                </div>
                <h3 class = "border-BS4 white--text">Self Study</h3>
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
                                                Have you ever driven a sports car?<br />
                                                Yes, I’ve driven a Porsche. My friend’s got one.<br />
                                                It was incredible!<br />
                                                It was amazing!<br />
                                                I was a bit scared though
                                            </p>
                                            <p>
                                                Some adjectives have two forms, one ending –ed, the other –ing.<br />
                                                Amazed/amazing : frightened/frightening : relaxed/relaxing : bored/boring : interested/interesting<br />
                                                Tired/tiring
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
              name:'Brendan:',
              speech:'You’ve done a parachute jump?'
            },
            {
              name:'Lisa:',
              speech:'Yeah.'
            },
            {
              name:'Brendan:',
              speech:'Seriously?'
            },
            {
              name:'Lisa:',
              speech:'Yeah!'
            },
            {
              name:'Brendan:',
              speech:'When?'
            },
            {
              name:'Lisa:',
              speech:'About… four years ago. A group of us went, from my last company.'
            },
            {
              name:'Brendan:',
              speech:'Wow! I’m impressed! So what was it like?'
            },
            {
              name:'Lisa:',
              speech:'Fantastic! When you jump out of the plane, it’s… it’s just amazing.'
            },
            {
              name:'Brendan:',
              speech:'You weren’t too scared, then?'
            },
            {
              name:'Lisa:',
              speech:'I was before I jumped. Everyone’s frightened before their first jump. But as soon as your parachute opens, it’s… it’s actually quite relaxing. You’re just there in the air – you’ve got this incredible view…'
            },
            {
              name:'Brendan:',
              speech:'Yeah, I bet. And what about the landing?'
            },
            {
              name:'Lisa:',
              speech:'It was OK. Not too hard.'
            },
            {
              name:'Brendan:',
              speech:'Because that’s the most dangerous moment, isn’t it?'
            },
            {
              name:'Lisa:',
              speech:'Well, yeah! Even if you jump without a parachute, it’s not dangerous until you land!'
            },
            {
              name:'Brendan:',
              speech:'No, good point!'
            },
            ],


            translations:[
            {
              name:'브렌던:',
              speech:'낙하산 점프를 했다고?'
            },
            {
              name:'리사:',
              speech:'그래.'
            },
            {
              name:'브렌던:',
              speech:'진짜로?'
            },
            {
              name:'리사:',
              speech:'그래!'
            },
            {
              name:'브렌던:',
              speech:'언제?'
            },
            {
              name:'리사:',
              speech:'약 4년 전에. 지난번 회사에서 우리 일행이 갔었어.'
            },
            {
              name:'브렌던:',
              speech:'와! 감동 받았어! 그래서 어땠어?'
            },
            {
              name:'리사:',
              speech:'환상적이야! 비행기에서 뛰어내리면 정말 놀라워.'
            },
            {
              name:'브렌던:',
              speech:'그럼 별로 안 무서웠나?'
            },
            {
              name:'리사:',
              speech:'내가 뛰어내리기 전엔 그랬어. 다들 첫 점프를 하기 전에 겁에 질려 있어 하지만 낙하산이 열리자 마자, 사실 꽤 편안해졌어. 당신은 그저 공중에 떠 있을 뿐인데, 믿을 수 없는 경치를 볼 수 있어.'
            },
            {
              name:'브렌던:',
              speech:'그래, 장담해. 착륙은?'
            },
            {
              name:'리사:',
              speech:'괜찮았어. 그다지 어렵지 않아.'
            },
            {
              name:'브렌던:',
              speech:'왜냐하면 그 순간이 가장 위험한 순간이기 때문이지, 안 그래?'
            },
            {
              name:'리사:',
              speech:'음, 그래! 낙하산 없이 뛰어내린다 해도 착륙할 때까지는 위험하지 않아!'
            },
            {
              name:'브렌던:',
              speech:'좋은 지적이야!'
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


</style>
