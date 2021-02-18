<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/laundromat-worker_1098-13867.jpg" class="cover-photo">

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
        padding-bottom: 10px;">It's Fantastic!
      </h1>
    </v-layout>

  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">It's Fantastic!</li><br />

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
          <u>Form a positive statement, a negative statement and a question</u><br />
              Ex) <br />
                  a) I've had lunch. <br />
                  b) I haven't had lunch.<br />
                  c) Have I had lunch?<br />
        </p>

        <ol style="margin: 12px;">
          <li>
            <br />
            (+) She washed the clothes.<br />
            (-) <u> &emsp; &emsp; &emsp; </u> <br/>
            (?) <u> &emsp; &emsp; &emsp; </u> <br/>
          </li>
          <br />
          <li>
            <br />
            (+) <u> &emsp; &emsp; &emsp; </u><br />
            (-) They haven't cleaned the house. <br/>
            (?) <u> &emsp; &emsp; &emsp; </u> <br/>
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
                      two piles of dirty clothes : 더러운 옷 두 더미<br />
                    </li>
                    <li>
                      the only difference : 유일하게 다른 점 <br />
                    </li>
                    <li>
                      while ... 진행형 : ~하는동안<br />
                    </li>
                    <li>
                      from now on : 이제부터<br />
                    </li>
                    <li>
                      we've ever used : 우리가 사용해본 적이 없다<br />
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
          name:'Brian Humble:',
          speech:'Meet Mr. and Mrs. Lopez of San Antonio, Texas. They have three young children, and they have to do a lot of wash.' +
          ' There are two piles of dirty clothes on this table. With this pile we’re going to use new Fizz, and with that pile we’re going to use another leading detergent.' +
          ' We have two identical washing machines here. The only difference is Fizz. While the machines are working, let’s have some coffee.'
        },
        {
          name:' ',
          speech:'OK, both machines have stopped, and Mr. Lopez has taken the clothes out. Well, Mr. Lopez, what do you think?'
        },
        {
          name:'Mr. L.:',
          speech:'Well, we washed these clothes with Fizz and those clothes with the other detergent.'
        },
        {
          name:'Brian:',
          speech:'Can you see any difference?'
        },
        {
          name:'Mr. L.:',
          speech:'I sure can! These clothes over here are much cleaner. And they’re whiter and softer than those over there.'
        },
        {
          name:'Brian:',
          speech:'These clothes? We washed these clothes with new Fizz!'
        },
        {
          name:'Mrs. L.:',
          speech:'That’s right, Brian. It’s really much better than our usual detergent. Our clothes have never been cleaner than this!'
        },
        {
          name:'Brian:',
          speech:'So, which detergent are you going to use from now on?'
        },
        {
          name:'Mr. L.:',
          speech:'New Fizz, of course. It’s the best detergent we’ve ever used!'
        },
        ],

        translations:[
        {
          name:'Brian Humble:',
          speech:'텍사스 샌안토니오의 Lopez부부를 만나보십시오. 그들에게는 세 명의 어린 자녀가 있는데, 그들은 많은 양의 씻기를 해야 한다.' +
          ' 이 탁자 위에는 더러운 옷 두 개가 쌓여 있다. 이 더미로 우리는 새로운 피즈를 사용할 것이고, 그 더미로 우리는 또 다른 선도적인 세제를 사용할 것이다.' +
          ' 여기 똑같은 세탁기가 두 대 있어. 유일한 차이점은 피즈다. 기계가 작동되는 동안, 커피를 마시자.'
        },
        {
          name:' ',
          speech:'좋아, 두 기계 모두 멈췄고, Lopez씨는 옷을 꺼내 입었어. 로페즈씨, 어떻게 생각하십니까?'
        },
        {
          name:'L씨:',
          speech:'음, 우리는 이 옷들을 피즈와 다른 세제로 세탁했어.'
        },
        {
          name:'Brian:',
          speech:'뭐가 다른지 알겠니?'
        },
        {
          name:'L씨:',
          speech:'난 정말 할 수 있어! 여기 이 옷들은 훨씬 깨끗하다. 그리고 그들은 저쪽에 있는 사람들보다 더 작고 부드럽다.'
        },
        {
          name:'Brian:',
          speech:'이 옷들? 우리는 이 옷들을 새 피즈로 빨았어!'
        },
        {
          name:'L씨 부인::',
          speech:'부인: 맞아, Brian . 우리 보통 세제보다 훨씬 더 맛있어. 우리 옷은 이보다 더 깨끗해진 적이 없어!'
        },
        {
          name:'Brian:',
          speech:'그래, 이제부터 어떤 세제를 사용할 거야??'
        },
        {
          name:'L씨:',
          speech:'물론 뉴 피즈. 지금까지 사용한 세제 중에 최고야!'
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
