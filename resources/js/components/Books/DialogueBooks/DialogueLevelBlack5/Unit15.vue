<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/cheerful-doctor-talking-with-elderly-patient_23-2147896869.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Guess what I’m thinking of
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br />( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Guess what I’m thinking of</li><br />
     
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
          <u>Combine the sentences</u><br />
        </p>
        <br />
        <p>
          A) WHOSE<br />
            Ex) We saw a woman. Her dog was bigger than she was. >> We saw a woman whose dog was bigger than she was.<br />
        </p>
        <br />
        <ol style="margin: 12px;">
          <li>
            They have a friend. His family is very rich.       >><br />
          </li>
          <li>
            He married a woman. Her favorite hobby is cooking.      >><br />
          </li>
          <li>
            I talked to a boy. His father is a salesman.      >> <br />
          </li>
        </ol>
        <br />

        <p>
          A) WHERE<br />
          Ex) Where can we play basketball?      >>    I know a good place where we can play basketball.<br />
        </p>
        <br />
        <ol style="margin: 12px;">
          <li>
            Where can I buy nice shoes? – I know …<br />
          </li>
          <li>
            Where can we have a picnic? – I know …<br />
          </li>
          <li>
            Where can I get a job? – I know … <br />
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
                      I’m thinking of a place where people have picnics (나는 사람들이 소풍을 하고 있는 장소를 생각하고 있다)<br />
                        -> I'm thinking of a place. + People have picnics there.<br />
                      I’m thinking of a restaurant where you can have great ice cream(나는 너가 대단 아이스크림을 먹을 수 있는 식당을 생각하고 있어)<br />
                        -> I'm thinking of a restaurant. + you can have great ice cream there.<br />
                    </li>
                    <li>
                      관계대명사 whose : 선행사가 사람일 때 사용되고, 선행사가 형용사절 안에서 소유격으로 쓰일 때 whose를 씁니다.<br />
                        Example:<br />
                          I’m thinking of a man whose favorite hobby is chasing butterflies. ( 나는 가장 좋아하는 취미가 나비 잡기는 남자를 생각하고 있어)<br />
                            -> I'm thinking of a man. + His favorite hobby is chasing butterflies.<br />
                          I’m thinking of a woman whose house is full of cats. (나는 집이 고양이로 가득찬 여자를 생각하고 있어)<br />       
                            -> I'm thinking of a woman. + Her house is full of cats.<br />     
                    </li>
                    <li>
                      guess what I’m thinking of : 내가 무엇을 생각하는지 추측해봐
                    </li>
                    <li>
                      must be : ~임에 틀림없다
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
          speech:'Andrew, let’s play a game. See if you can guess what I’m thinking of.'
        },
        {
          name:'B:',
          speech:'Okay. Go ahead.'
        },
        {
          name:'A:',
          speech:'I’m thinking of a man whose favorite hobby is chasing butterflies.'
        },
        {
          name:'B:',
          speech:'That’s easy. Dr. Hill.'
        },
        {
          name:'A:',
          speech:'I’m thinking of a woman whose house is full of cats'
        },
        {
          name:'B:',
          speech:'That must be Mrs. Johnson.'
        },
        {
          name:'A:',
          speech:'Now I’m thinking of a place where people have picnics.'
        },
        {
          name:'B:',
          speech:'I know. City Park.'
        },
        {
          name:'A:',
          speech:'I’m thinking of a restaurant where you can have great ice cream.'
        },
        {
          name:'B:',
          speech:'That must be the Martinoli Restaurant.'
        },
        {
          name:'A:',
          speech:'Very good, Andrew. You guessed them all. Can you guess what I want to do now?'
        },
        {
          name:'B:',
          speech:'Sure, you want to have ice cream at the Martinoli Restaurant. Let’s go.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'Andrew, 게임을 해요. 제가 무슨 생각을 하는지 아시겠어요?'
        },
        {
          name:'B:',
          speech:'알았어요. 말씀 계속하세요'
        },
        {
          name:'A:',
          speech:'나비를 쫓는 게 취미인 남자를 생각하고 있어요.'
        },
        {
          name:'B:',
          speech:'그건 쉬워요. Dr. Hill입니다'
        },
        {
          name:'A:',
          speech:'집이 고양이들로 가득 찬 여자를 생각하고 있어요.'
        },
        {
          name:'B:',
          speech:'Johnson부인인가 봐요.'
        },
        {
          name:'A:',
          speech:'지금은 사람들이 소풍을 가는 곳을 생각하고 있어요.'
        },
        {
          name:'B:',
          speech:'알아요. 도시 공원입니다.'
        },
        {
          name:'A:',
          speech:'맛있는 아이스크림을 먹을 수 있는 식당을 생각하고 있어요.'
        },
        {
          name:'B:',
          speech:'저기가 Martinoli 식당인가 봐요.'
        },
        {
          name:'A:',
          speech:'좋아요, Andrew. 다 맞혔잖아요. 내가 지금 무엇을 하고 싶은지 추측할 수 있나요?'
        },
        {
          name:'B:',
          speech:'물론이죠, Martinoli 식당에서 아이스크림을 드시고 싶을 거예요. 가죠.'
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
