<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/beautiful-smart-asian-doctor-patient-discussing-explaining-something-with-clipboard_7861-1219.jpg" class="cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgb(59, 105, 120, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Judy at the hospital
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Judy at the hospital</li><br />
      <br />
      <p>
        Last Sunday Judy had a lot of visitors, and they brought her some nice presents. At the end of the day Rachel came by and the two women had a pleasant talk.<br />
      </p>
      <br />
      <table style = "border-collapse: collapse;">
    
        <tr v-for="dialog in dialogs" :key="dialog">
          <td class = "uppertable" >{{dialog.name}}</td>
          <td class = "lowertable" >{{dialog.speech}}</td>
        </tr>
  
      </table>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;
                                              margin-left: -18px;
                                              margin-right: -18px;
                                              padding-left: 10px;
                                              padding-bottom: 10px;
                                              padding-top: 10px;
                                              margin-top: 0px;
                                              background-color: #204051;">Exercise</h3>
        <div style="padding : 16px;">

        <p>
          <u>Answer the questions</u><br />
        </p>

        <ol style="margin: 12px;">
          <li>
            Who gave Judy the pictures?
          </li>
          <li>
            Will Judy be able to fly again soon?
          </li>
          <li>
            Why does she have to go home next week?
          </li>
        </ol>

      <p>
        Free response:<br />
        Is there anything in your life that you really regret?<br />
      </p>
      </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;
                                              margin-left: -18px;
                                              margin-right: -18px;
                                              padding-left: 10px;
                                              padding-bottom: 10px;
                                              padding-top: 10px;
                                              margin-top: 0px;
                                              background-color: #204051;">Translation</h3>
      <div style="padding : 16px;">

        <p>
          지난 일요일 Judy 는 많은 방문객을 맞이했고 그들은 그녀에게 멋진 선물을 가져다 주었습니다. 급기야 Rachel 이 들렀고 두 여자는 즐거운 대화를 나누었습니다.<br />
        </p>

        <table style = "border-collapse: collapse;">

          <tr v-for="translation in translations" :key="translation">
            <td class = "uppertable" >{{translation.name}}</td>
            <td class = "lowertable" >{{translation.speech}}</td>
          </tr>
  
        </table>

</div>
        <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
        </div>
        <h3 class = "border white--text" style="padding-top: 7px;
                                                margin-left: -18px;
                                                margin-right: -18px;
                                                padding-left: 10px;
                                                padding-bottom: 10px;
                                                padding-top: 10px;
                                                margin-top: 0px;
                                                background-color: #204051;">Self Study</h3>
        <div style="padding : 16px;">

          <p>

            <v-container grid-list-md text-xs-left>
              <v-layout row wrap>


                <v-flex xs12>
                  <v-card light color="#cae8d5">
                    <v-card-text class="px-10">
                    <li>
                      Notes
                    </li>
                    <ol style="margin: 12px;">
                    <li>
                      수여동사 bring : 주어+bring+간접목적어+직접목적어<br />
                      Ex) She brought me a box of chocolates : 그녀는 나에게 초콜렛 한 박스를 가져왔다 Expressions.                   
                    </li>
                    <li>
                      at the end of the day : 마지막 날에
                    </li>
                    <li>
                      have a pleasant talk : 유쾌한 대화를 나누다
                    </li>
                    <li>
                      come by (~의 곁을) 지나다. ~을 손에 넣다
                    </li>
                    <li>
                      a little while ago : 방금 전에
                    </li>
                    <li>
                      take advantage of : ~을 이용하다, ~편승하다
                    </li>
                    <li>
                      "I may not be able to help Matt anymore with his campaign for mayor" : 나는 더이상 Matt의
                    </li>
                    <li>
                      장 유세를 도와줄 수 없을지도 모른다
                    </li>
                    <li>
                      "it means so much to me" : 그것은 내게 큰 의미가 된다
                    </li>
                    <li>
                      for quite a while : 한동안, 오랫동안
                    </li>
                    <li>
                      "it’s up to you" : 그것은 너에게 달려 있다
                    </li>
                    </ol>
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

  data(){

    return{
        dialogs:[
        {
          name:'A:',
          speech:'How are you feeling today?'
        },
        {
          name:'B:',
          speech:'Much better. A lot of people came to see me this weekend, and look at all the nice things they brought.'
        },
        {
          name:'A:',
          speech:'Those pictures look interesting. May I see them?'
        },
        {
          name:'B:',
          speech:'Of course. Aren’t they beautiful? Fred gave them to me.'
        },
        {
          name:'A:',
          speech:'That’s nice of him. Who else came to see you this weekend?'
        },
        {
          name:'B:',
          speech:'Well, Anne was here yesterday. She brought me a box of chocolates. And Matt came by a little while ago with some magazines and a book.'
        },
        {
          name:'A:',
          speech:'That was a good idea. You might as well take advantage of this opportunity and do some reading.'
        },
        {
          name:'B:',
          speech:'You’re right. My only regret is that I may not be able to help Matt anymore with his campaign for mayor. It means so much to me.'
        },
        {
          name:'A:',
          speech:'You won’t be able to fly your plane again for quite a while, if that’s what you mean.'
        },
        {
          name:'B:',
          speech:'There’s something else that worries me. My insurance only covers the first week I’m in the hospital, and I’ve already been here for five days. Do you think I might be able to stay with my family next week?'
        },
        {
          name:'A:',
          speech:'It’s up to you. But please talk to me again before you do anything.'
        },
        {
          name:'B:',
          speech:'You can count on it. Thanks for everything, Rachel.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'오늘 기분 어때요?'
        },
        {
          name:'B:',
          speech:'훨씬 낫습니다. 이번 주말에 많은 사람들이 저를 보러 왔고, 그들이 가져온 좋은 것들을 보세요.'
        },
        {
          name:'A:',
          speech:'그 사진들이 재미있어 보이네요. 제가 그들을 봐도 될까요?'
        },
        {
          name:'B:',
          speech:'물론이죠. 아름답지 않나요? Fred 가 저에게 줬어요.'
        },
        {
          name:'A:',
          speech:'정말 친절하시네요. 이번 주말에 또 누가 당신을 보러 왔습니까?'
        },
        {
          name:'B:',
          speech:'음, Anne 은 어제 여기 있었어요. 그녀는 나에게 초콜릿 한 상자를 가져왔습니다. 그리고 Matt 는 조금 전에 잡지와 책을 가지고 왔습니다.'
        },
        {
          name:'A:',
          speech:'좋은 생각이었어요. 당신은 이 기회를 이용해서 독서를 하는 게 좋겠어요.'
        },
        {
          name:'B:',
          speech:'맞아요. 제 유일한 유감은 제가 더 이상 Matt 의 시장 선거 운동을 도울 수 없을지도 모른다는 것입니다. 나한테 정말 뜻깊은 일이었어요.'
        },
        {
          name:'A:',
          speech:'그런 뜻이라면 꽤 오랫동안 비행기를 다시 조종할 수 없을 거예요.'
        },
        {
          name:'B:',
          speech:'다른 걱정거리가 있어요. 제 보험은 제가 입원한 첫 주에만 적용되는데, 벌써 5일이나 입원했어요. 제가 다음 주에 가족과 함께 지낼 수 있을까요?'
        },
        {
          name:'A:',
          speech:'그건 당신에게 달렸어요. 하지만 당신이 무슨 일을 하기 전에 저에게 다시 말해주세요.'
        },
        {
          name:'B:',
          speech:'믿어도 돼요. 고마워요, Rachel.'
        },
        ]

    }

  },


  beforeMount(){


  },

  methods:{


  },

  watch:{

    fontSize(current, old){

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
  border-color: transparent #204051 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background: #204051;
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
