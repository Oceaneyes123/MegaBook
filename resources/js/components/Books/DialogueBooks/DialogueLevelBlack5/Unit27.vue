<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/young-guy-aged-man-sitting-sofa_23-2148030251.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Joining the army
        </h1>
    </v-layout>

  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Joining the army</li><br />

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
            Do all young men in Korea have served in the army?
          </li>
          <li>
            How long do they have to serve?
          </li>
          <li>
            Do they go to the army right after graduating from high school or after they graduate from college?
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
                      조동사 have to : 미래의 의무와 필요를 나타낼 때에는 will have to (긍정, ~해야만 할 것이다), won't have to (부정, ~할 필요는 없을 것이다)<br />   
                          Example:<br />
                              You’ll have to cut your hair : 머리를 잘라야 할 것이다<br /> 
                              You won't have to wear it too short : 너무 짧게 할 필요는 없을 것이다<br /> 
                              You’ll have to eat a lot of beans, but at least you won’t have to do the cooking : 많은 콩을 먹어야 할 것이다 하지만 적어도 요리는 하지 않아도 될 것이다 <br />
                              You’ll have to do a lot of marching : 너는 많은 행군을 해야만 할거야<br/>
                    </li>
                    <li>
                      join the army : 군에 가다
                    </li>
                    <li>
                      graduate from : ~을 졸업하다
                    </li>
                    <li>
                      "What’ll it be like if I join the army?" : 군에 간다면 어떨까요?
                    </li>
                    <li>
                      first of all : 무엇보다도, 먼저, 우
                    </li>
                    <li>
                      make a decision : 결정하다
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
          speech:'Dad, I want to ask you something.'
        },
        {
          name:'B:',
          speech:'Sure. What is it, son?'
        },
        {
          name:'A:',
          speech:'Do you think I should join the army after I graduate from high school?'
        },
        {
          name:'B:',
          speech:'Well, you don’t have to join the army, but you should do something for your country.'
        },
        {
          name:'A:',
          speech:'What’ll it be like if I join the army?'
        },
        {
          name:'B:',
          speech:'First of all, you’ll have to cut your hair. But you won’t have to wear it too short.'
        },
        {
          name:'A:',
          speech:'Will the food be OK?'
        },
        {
          name:'B:',
          speech:'Ha! Ha! You’ll have to eat a lot of beans, but at least you won’t have to do the cooking.'
        },
        {
          name:'A:',
          speech:'Will I have to carry a rifle?'
        },
        {
          name:'B:',
          speech:'Of course, and you’ll have to do a lot of marching. But that won’t hurt you.'
        },
        {
          name:'A:',
          speech:'What are the advantages of joining the army?'
        },
        {
          name:'B:',
          speech:'You can learn a lot, son. You’ll have to work hard, but it’s a good experience. And when you get out, you’ll be ready for college.'
        },
        {
          name:'A:',
          speech:'That sounds pretty good. I’m going to give it some more thought before I make a decision.'
        },
        {
          name:'B:',
          speech:'Sure, Jimmy. Take your time and then decide.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'아빠, 물어볼 게 있어요.'
        },
        {
          name:'B:',
          speech:'왜 그래, 아들?'
        },
        {
          name:'A:',
          speech:'고등학교 졸업 후에 군대에 가야 할까요?'
        },
        {
          name:'B:',
          speech:'음, 군대에 갈 필요는 없지만, 조국을 위해 뭔가를 해야 해.'
        },
        {
          name:'A:',
          speech:'군대에 가면 어떻게 될까요?'
        },
        {
          name:'B:',
          speech:'우선 머리를 잘라야 할 거야. 하지만 너무 짧게 입을 필요는 없을 거야.'
        },
        {
          name:'A:',
          speech:'음식이 괜찮을까요?'
        },
        {
          name:'B:',
          speech:'하! 하! 콩을 많이 먹어야 할 텐데, 적어도 요리는 안 해도 될 거야.'
        },
        {
          name:'A:',
          speech:'라이플총을 들고 다녀야 하나요?'
        },
        {
          name:'B:',
          speech:'물론, 그리고 행군도 많이 해야 할 거야. 하지만 그건 너에게 해가 되지 않을 거야'
        },
        {
          name:'A:',
          speech:'군대에 가면 어떤 장점이 있나요?'
        },
        {
          name:'B:',
          speech:'많이 배울 수 있어, 아들아. 열심히 해야겠지만 좋은 경험이야 그리고 너가 나오면,  대학에 갈 준비가 될 거야..'
        },
        {
          name:'A:',
          speech:'그거 꽤 괜찮은 것 같은데요. 결정을 내리기 전에 좀 더 생각해 볼게요.'
        },
        {
          name:'B:',
          speech:'그럼, Jimmy. 천천히 결정해.'
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
