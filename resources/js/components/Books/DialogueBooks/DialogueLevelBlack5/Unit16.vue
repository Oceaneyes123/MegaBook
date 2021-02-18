<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/businessman-sitting-armchair_155003-11435.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Role in a movie
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Role in a movie</li><br />

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
          <u>Complete the sentences</u><br />
          Ex) Who is that man? > Do you know who that man is?<br />
        </p>

        <ol style="margin: 12px;">
          <li>
            How much does this book cost?  >  Can you tell me <u> &emsp; &emsp; &emsp; </u><u> &emsp; &emsp; &emsp; </u>?<br />
          </li>
          <li>
            What did you say?  >  I didn’t hear <u> &emsp; &emsp; &emsp; </u><u> &emsp; &emsp; &emsp; </u>.<br />
          </li>
          <li>
            Where did I leave the key?  >  I can’t remember <u> &emsp; &emsp; &emsp; </u><u> &emsp; &emsp; &emsp; </u>.<br />
          </li>
          <li>
            Why are you so upset?  >  I don’t understand <u> &emsp; &emsp; &emsp; </u><u> &emsp; &emsp; &emsp; </u>.<br />
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
                      간접의문문 : 의문문이 다른 문장의 일부로 포함되어 있을 때, 이것을 간접의문문이라고 합니다. 간접의문문에 의문사 뒤의 어순은 '주어 + 동사' 이고 앞 문장의 동사의 목적어역할을 합니다.<br />                 
                        a) 의문사가 있는 간접의문문 : 의문사가 있는 의문문이 다른 문장의 일부로 포함될 때, '의문사 + 주어 + 동사' 로 바뀝니다.<br />
                          Example:<br />
                              Do you know where he went? (당신은 그가 어디 갔는지 알고 있습니까?)<br />
                                -> Do you know? + Where did he go?<br />
                              Do you know how Fred met her? (당신은 어떻게 Fred가 그녀를 만나지 아십니까? <br />
                                -> Do you know? + How did Fred meet her?<br />
                              I wonder what she's doing here. (나는 그녀가 여기서 무엇을 하는지 알고 싶다)<br />  
                                -> I wonder. + What is she doing here?<br />
                              I wonder why she wants Fred. (나는 그녀가 왜 Fred를 필요로 하는지 궁금하다)<br /> 
                                -> I wonder. + Why does she want Fred?<br />
                        b) 의문문사가 없는 간접의문문 : 의문사가 없는 의문문이 다른 문장의 일부로 포함될 때, 'if(~인지 아닌지) + 주어 + 동사' 로 바뀝니다. I wonder if she needs someone like me. (나는 그녀가 나같은 누군가를 필요로 하는지 궁금하다) <br />                
                                -> I wonder. + Does she need someone like me?<br />
                      </li>
                    <li>
                      "she came for a little rest" : 그녀는 잠시 쉬러 왔다
                    </li>
                    <li>
                      according to ~ : ~에 따르면
                    </li>
                    <li>
                      have experience : 경험이 있다
                    </li>
                    <li>
                      it isn’t necessary : 필연적이지 않다
                    </li>
                    <li>
                      "he’s going to play the role of a taxi driver" : 그는 택시 운전사의 역할을 할 예정이다
                    </li>
                    <li>
                      anything is possible : 무엇이든 가능하다
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
          speech:'Hi, Nick. Have you seen Fred?'
        },
        {
          name:'B:',
          speech:'Yes, he was here this morning.'
        },
        {
          name:'A:',
          speech:'Do you know where he went?'
        },
        {
          name:'B:',
          speech:'The Plaza Hotel. He went to see Angela Joule, the famous movie star.'
        },
        {
          name:'A:',
          speech:'Angela Joule? I didn’t know she was in the city. I wonder what she’s doing here.'
        },
        {
          name:'B:',
          speech:'Fred says she came for a little rest. She likes the peace and quiet of our town.'
        },
        {
          name:'A:',
          speech:'Oh, I see. Do you know how Fred met her?'
        },
        {
          name:'B:',
          speech:'She took his taxi at the airport a few days ago.'
        },
        {
          name:'A:',
          speech:'Why did he go to see her at the hotel?'
        },
        {
          name:'B:',
          speech:'Well, according to Fred, she has a part for him in her new movie.'
        },
        {
          name:'A:',
          speech:'I wonder why she wants Fred. He’s never had any acting experience.'
        },
        {
          name:'B:',
          speech:'It isn’t necessary. He’s going to play the role of a taxi driver.'
        },
        {
          name:'A:',
          speech:'Hmm. I wonder if she needs someone like me.'
        },
        {
          name:'B:',
          speech:'You never know, Frankie. Anything is possible.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'안녕하세요, Nick. Fred 봤어요?'
        },
        {
          name:'B:',
          speech:'네, 그는 오늘 아침에 여기 있었어요.'
        },
        {
          name:'A:',
          speech:'그 사람이 어디로 갔는지 아세요?'
        },
        {
          name:'B:',
          speech:'플라자 호텔입니다. 그는 유명한 영화배우인 Angela Joule을 보러 갔습니다.'
        },
        {
          name:'A:',
          speech:'Angela Joule이라고요? 저는 그녀가 도시에 있는지 몰랐어요. 저는 그녀가 여기서 무엇을 하고 있는지 궁금해요.'
        },
        {
          name:'B:',
          speech:'Fred 가 좀 쉬러 왔다고 하네요. 그녀는 우리 마을의 평화와 고요함을 좋아합니다.'
        },
        {
          name:'A:',
          speech:'아, 그렇군요. Fred 가 어떻게 그녀를 만났는지 아세요?'
        },
        {
          name:'B:',
          speech:'그녀는 며칠 전에 공항에서 그의 택시를 탔어요.'
        },
        {
          name:'A:',
          speech:'그는 왜 호텔로 그녀를 만나러 갔나요?'
        },
        {
          name:'B:',
          speech:'음, Fred 에 따르면, 그녀는 그녀의 새 영화에서 그를 위한 배역이 있다고 해요.'
        },
        {
          name:'A:',
          speech:'왜 그녀가 Fred 를 원하는지 궁금하네요. 그 사람은 연기 경험이 없어요.'
        },
        {
          name:'B:',
          speech:'그럴 필요는 없어요. 그는 택시 운전사 역할을 할 거예요.'
        },
        {
          name:'A:',
          speech:'음. 그녀가 나 같은 사람이 필요한지 궁금해요'
        },
        {
          name:'B:',
          speech:'절대 모르잖아요, Frankie. 무엇이든 가능합니다.'
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
