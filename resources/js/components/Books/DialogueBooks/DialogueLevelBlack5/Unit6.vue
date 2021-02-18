<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/group-creative-friends-sitting-wooden-table-people-were-having-fun-while-playing-board-game_146671-15242.jpg" class="cover-photo">

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
        padding-bottom: 10px;">The trivia game
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">The trivia game</li><br />

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
            Which city is the biggest in Korea? What is its population? <br />
          </li>
          <li>
            What is the highest mountain in Korea?<br />
          </li>
          <li>
            What's the most beautiful place in Korea?<br />
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
                      최상급 만들기 : 보통 형용사나 부사 뒤에 est를 붙이거나 앞에 most를 넣어 나타냅니다. most는 2음절어의 대부분, (-ful, -ous, -ive, -ing, -ed)등으로 끝나는 단어와 3음절 이상의 단어에 붙입니다.<br />
                          big   >   the biggest<br />
                          small   >   the smallest<br />
                          intelligent   >   the most intelligent<br />                  
                    </li>
                    <li>
                      최상급 비교 구문 : 보통 앞에 the가 오고 뒤에는 of(~중에서)나 in(~안에서) 등 한정해 주는 말이 오는 경우가 많습니다.<br />
                      the 최상급 + in + 장소나 범위를 나타내는 단수 명사 (the world, the class, the team등) : ~ 안에서 가장 ~한<br />
                      the 최상급 + of + 비교 대상이 되는 복수 명사 (friends, singers등) : ~ 중에서 가장 ~한 <br />
                      the 최상급 + (that) 주어 + have ever v-ed : 주어가 지금까지 ~한 것들 중에 가장 ~한<br />         
                    </li>
                    <li>
                      최상급 강조 : much, by far, the very등을 씁니다.<br />
                    </li>
                    <li>
                      It's my turn : 내 차례야<br />
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
          speech:'OK. It’s my turn. Three. One, two, three. I’m on blue.'
        },
        {
          name:'B:',
          speech:'Blue. That’s Geography. What’s the biggest country in the world?'
        },
        {
          name:'A:',
          speech:'Uh, Canada.'
        },
        {
          name:'B:',
          speech:'No. Russia’s bigger than Canada. It’s the biggest country in the world.'
        },
        {
          name:'A:',
          speech:'That’s not right! In my geography book, the U.S.S.R. was the biggest, but Russia is smaller than the U.S.S.R..'
        },
        {
          name:'B:',
          speech:'It doesn’t matter, Candice. Russia is smaller than the U.S.S.R., but it’s still bigger than Canada. Next question.'
        },
        {
          name:'A:',
          speech:'OK. Six! What’s that?'
        },
        {
          name:'B:',
          speech:'Nature. What is the most intelligent animal in the world?'
        },
        {
          name:'A:',
          speech:'That’s easy. Humans are the most intelligent.'
        },
        {
          name:'B:',
          speech:'No.'
        },
        {
          name:'A:',
          speech:'What do you mean, "no"?'
        },
        {
          name:'B:',
          speech:'The answer on the card is whales. Whales have the biggest brains.'
        },
        {
          name:'A:',
          speech:'But that’s not the same thing'
        },
        {
          name:'B:',
          speech:'That’s the answer on the card. OK, it’s my turn.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'좋아요. 이제 제 차례에요. 셋. 하나, 둘, 셋. 파란색이에요.'
        },
        {
          name:'B:',
          speech:'파란색. 그건 지리학입니다. 세계에서 가장 큰 나라는 어디인가요?'
        },
        {
          name:'A:',
          speech:'음, 캐나다요.'
        },
        {
          name:'B:',
          speech:'아니요. 러시아는 캐나다보다 더 큽니다. 세계에서 가장 큰 나라입니다.'
        },
        {
          name:'A:',
          speech:'그건 옳지 않아요! 제가 쓴 지리학 책에서는 미국이 가장 크지만 러시아는 미국보다 작습니다.'
        },
        {
          name:'B:',
          speech:'상관없어요, Candice. 러시아는 미국보다 작지만, 여전히 캐나다보다 큽니다. 다음 질문입니다.'
        },
        {
          name:'A:',
          speech:'좋아요. 여섯! 저건 뭐예요?'
        },
        {
          name:'B:',
          speech:'자연입니다. 세상에서 가장 똑똑한 동물은 무엇일까요?'
        },
        {
          name:'A:',
          speech:'그건 쉬워요. 인간은 가장 총명합니다.'
        },
        {
          name:'B:',
          speech:'아니요.'
        },
        {
          name:'A:',
          speech:'안 된다는 게 무슨 뜻이에요?'
        },
        {
          name:'B:',
          speech:'카드의 답은 고래입니다. 고래는 가장 큰 뇌를 가지고 있습니다.'
        },
        {
          name:'A:',
          speech:'하지만 그건 달라요!'
        },
        {
          name:'B:',
          speech:'그게 답이에요. 좋아요, 이제 제 차례에요.'
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
