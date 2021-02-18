<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/side-view-screaming-happy-bearded-man-business-clothes_171337-11389.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Big chance
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Big chance</li><br />
      <br />
      <p>
        Fred loved talking and made the most of his opportunity when Miss Joule asked him to tell her about himself. He started telling Miss Joule about his experiences as a taxi driver. His favorite story was about a grandma who didn’t have any money and tried to pay her fare with chicken eggs. Miss Joule just sat back and listened. It was fascinating. After a while she leaned forward.<br />
      </p>
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
            What is Fred’s favorite story?<br />
          </li>
          <li>
            Why did Fred get the ticket?<br />
          </li>
        </ol>

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
          Fred는 말을 하는 것을 좋아했고, Joule 양이 자신에 대해 말해달라고 부탁했을 때 기회를 최대한 활용했습니다. 그는 Joule양에게 택시 운전사로서의 경험에 대해 말하기 시작했습니다. 그가 가장 좋아하는 이야기는 돈이 없어서 계란으로 요금을 내려고 하는 할머니에 대한 이야기이다. Joule 양은 그냥 뒤로 물러서서 듣고만 있었습니다. 정말 흥미로웠어요. 잠시 후 그녀는 몸을 앞으로 숙였습니다.<br />
        </p>
        <br />
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
                      made the most of : ~을 십분 이용하다 (Fred made the most of his opportunity : Fred는 그의 기회를 십분 이용했습니다)
                    </li>
                    <li>
                      experiences as a taxi driver : 택시 운전자로서의 경험
                    </li>
                    <li>
                      story about : ~에 관한 이야기
                    </li>
                    <li>
                      pay with : ~로 지불하다
                    </li>
                    <li>
                      sit back : ~에 깊숙이 앉다
                    </li>
                    <li>
                      ever since I was a little boy : 내가 어릴 적 부터
                    </li>
                    <li>
                      you went right through it : 당신은 바로 지나가 버렸습니다
                    </li>
                    <li>
                      play the part of : ~의 역할을 하다
                    </li>
                    <li>
                      I've always wanted to be ... : 나는 항상 ~이기를 원했다
                    </li>
                    <li>
                      Now’s my chance : 지금이 나의 기회이다
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
          name:'Joule:',
          speech:'Fred, you enjoy telling stories, don’t you?'
        },
        {
          name:'Fred:',
          speech:'Yes, ma’am. I’ve been telling stories ever since I was a little boy.'
        },
        {
          name:'Joule:',
          speech:'Well, I hope you’ve got a good one for the police officer right behind us.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'경찰관:',
          speech:'Didn’t you see the light back there?'
        },
        {
          name:'Fred:',
          speech:'What light, officer?'
        },
        {
          name:'경찰관:',
          speech:'The stop light at the intersection. You went right through it.'
        },
        {
          name:'Fred:',
          speech:'I … uh …'
        },
        {
          name:'경찰관:',
          speech:'I’m going to have to give you a ticket.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Joule:',
          speech:'Cheer up. You know what? I’ve got an offer for you.'
        },
        {
          name:'Fred:',
          speech:'What’s that?'
        },
        {
          name:'Joule:',
          speech:'I’ve just started making a new movie. We’re looking for someone who can play the part of a taxi driver. Would you like to do it?'
        },
        {
          name:'Fred:',
          speech:'Of course! I’ve always wanted to be in the movies. Now’s my chance.'
        },
        ],

        translations:[
        {
          name:'Joule:',
          speech:'Fred, 당신은 이야기를 하는 것을 즐기죠, 그렇죠?'
        },
        {
          name:'Fred:',
          speech:'네, 부인. 저는 어렸을 때부터 이야기를 해왔어요.'
        },
        {
          name:'Joule:',
          speech:'음, 우리 바로 뒤에 경찰관을 위한 좋은 것이 있었으면 좋겠어요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'경찰관:',
          speech:'저 뒤에 불빛이 보이지 않았나요?'
        },
        {
          name:'Fred:',
          speech:'무슨 빛이죠, 경관님?'
        },
        {
          name:'경찰관:',
          speech:'교차로의 정지 신호등입니다. 당신은 그것을 바로 통과했어요.'
        },
        {
          name:'Fred:',
          speech:'저는… 어…'
        },
        {
          name:'경찰관:',
          speech:'과태료 딱지를 드려야겠어요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Joule:',
          speech:'힘내요. 그거 알아요? 당신에게 제안할 게 있어요.'
        },
        {
          name:'Fred:',
          speech:'그게 뭐예요?'
        },
        {
          name:'Joule:',
          speech:'저는 이제 막 새로운 영화를 만들기 시작했어요. 택시기사 역할을 할 수 있는 사람을 찾고 있습니다. 하시겠어요?'
        },
        {
          name:'Fred:',
          speech:'물론이죠! 저는 항상 영화에 출연하고 싶었어요. 지금이 제 기회에요.'
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
