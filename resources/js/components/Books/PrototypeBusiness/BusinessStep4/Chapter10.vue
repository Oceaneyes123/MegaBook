<template>
<div :style="{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

        <v-layout column>
            <v-img src="https://marketplace.canva.com/MADGvx9A7cE/7/screen_2x/canva-file-arrangement-MADGvx9A7cE.jpg" class = "cover-photo">

                <v-layout align-end fill-height pa-0 white--text>
                    <h1 style="background-color: rgba(107, 190, 242, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing ideas 
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
                        Complete the second conditional sentences. Use the correct forms of the verbs.
                    </p>


                    <ol style="margin: 12px;">
                        <li>
                            If CDs <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> didn't have <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> packaging, they <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> would be <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u>
                            cheaper. (not have, be)
                        </li>
                        <li>
                            Our CDs <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> more if they <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> cheaper. (sell, be)
                        </li>
                        <li>
                            If we <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> the price, we <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> more CDs. (lower, sell)
                        </li>
                        <li>
                            I think we <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> more CDs if we <u>&emsp; &emsp; &emsp; &emsp; &emsp; </u> them in bigger packs. (sell,sell)
                        </li>
                    </ol>

                    <p>
                        Free response:<br />
                        Talk about creativity.<br />
                        How creative are you?<br />
                        How important is creativity for your work?<br />
                        Do you use your creative skills enough?
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
                                                Second conditional<br />
                                                <b>If</b> we <b>did</b> that, we’<b>d</b> have problems.(we’d = we would)<br />
                                                <b>If</b> we <b>used</b> plastic, we <b>could</b> make it lighter.
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
                name:'A:',
                speech:'OK, so our objective is to think of some new ideas. How could we make the product better? What areas of the product could we improve? Any suggestions?'
                },
                {
                name:'B:',
                speech:'What about changing the packaging? We could change the material.'
                },
                {
                name:'A:',
                speech:'Yeah. Packaging material. OK.'
                },
                {
                name:'C:',
                speech:'How about changing the size?'
                },
                {
                name:'A:',
                speech:'Of the CD?'
                },
                {
                name:'C:',
                speech:'No, the pack. Why don’t we sell more CDs in a pack, for example?'
                },
                {
                name:'A:',
                speech:'OK. Yeah. So, bigger packs. They could be smaller, as well.'
                },
                {
                name:'B:',
                speech:'Why not sell big boxes – big storage boxes, with lots of CDs in them? Then you wouldn’t need packaging.'
                },
                {
                name:'A:',
                speech:'So that would be a new product. A storage box.'
                },
                {
                name:'C:',
                speech:'We could sell CDs with numbers printed on them – say from one to a hundred. Then you wouldn’t need to write on the CD. You could make a note of what was on each CD number,and then find it easily. So we could sell, say, packs of ten. So you would have one to ten, or eleven to twenty, and so on.'
                },
                {
                name:'B:',
                speech:'That’s a good idea. We could use that idea with the storage box. So we could produce a big plastic box with, say, a hundred blank CDs in it, with the CDs numbered one to a hundred.'
                },
                {
                name:'A:',
                speech:'Mmm, that’s a, that’s an interesting idea.'
                },
            ],

            translations:[
            {
                name:'A:',
                speech:'좋아요. 우리의 목표는 새로운 아이디어를 생각해 보는 것입니다. 어떻게 하면 우리가 제품을 더 좋게 만들 수 있을까요? 제품의 어떤 부분을 개선할 수 있을까요? 좋은 의견이라도 있어요?'
                },
                {
                name:'B:',
                speech:'포장을 바꾸는 건 어때요? 우리는 재료를 바꿀 수 있습니다.'
                },
                {
                name:'A:',
                speech:'그래요. 포장재. 좋아요'
                },
                {
                name:'C:',
                speech:'사이즈를 바꾸는 건 어때요?'
                },
                {
                name:'A:',
                speech:'CD요?'
                },
                {
                name:'C:',
                speech:'아니요, 그 팩이요. 예를 들어 한 팩에 CD를 더 많이 파는 게 어때요?'
                },
                {
                name:'A:',
                speech:'좋아요. 네. 더 큰 팩. 그것들은 더 작을 수도 있습니다.'
                },
                {
                name:'B:',
                speech:'CD가 많이 들어 있는 큰 상자, 즉 큰 저장 상자를 팔면 어떨까요? 그럼 포장이 필요 없겠네요.'
                },
                {
                name:'A:',
                speech:'그럼 그건 새 제품인 거군요. 보관함.'
                },
                {
                name:'C:',
                speech:'1개에서 100개까지 번호가 인쇄된 CD를 판매할 수 있습니다. 그럼 당신은요 CD에 쓸 필요가 없어요 각 CD 번호에 있는 내용을 메모한 다음 쉽게 찾을 수 있을 거예요 그래서 우리는 열 개씩 팔 수 있을거예요. 1개에서 10 또는 11개에서 20개요.'
                },
                {
                name:'B:',
                speech:'좋은 생각이에요. 보관함와 함께 그 아이디어를 사용할 수 있습니다. 그래서 우리는 100개의 빈 CD가 들어 있는 큰 플라스틱 박스를 만들 수 있어요. CD의 숫자는 1에서 100까지입니다.'
                },
                {
                name:'A:',
                speech:'음, 그거 흥미로운 생각이네요.'
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
