<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/young-male-friends-having-morning-breakfast-home_23-2148195299.jpg" class="cover-photo">

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
        padding-bottom: 10px;">A new job
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">A new job</li><br />
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
            What do you like doing on weekends? / on vacations?<br />
          </li>
          <li>
            What do you enjoy doing in summer? / winter?<br />
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
                      동명사 (전치사의 목적어로 쓰이는 경우) : 전치사 뒤에는 명사가 나와야 하므로, 전치사 뒤에 동사가 나오면 동명사로 바꾸어 주어야 합니다. 이 때 전치사 뒤에 나온 동명사를 전치사의 목적어라고 합니다.<br />
                          Ex) I'm not interested in finding a new job : 나는 새 직업을 찾는 것에 흥미가 없다<br />
                              I'm already tired of doing the same thing every day : 나는 벌써 매일 같은 것을 하는 것에 지쳤다<br />
                              I'm afraid of getting really bored : 나는 정말 지루해지는 것이 두렵다<br />
                              I'm not interested in making more money : 나는 돈 버는 것에 흥미가 없다<br />
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
          name:'Patti:',
          speech:'Jeff, have you seen this ad in The New York Sentinel?'
        },
        {
          name:'Jeff:',
          speech:'Yes, I saw it, but I’m not interested in finding a new job. I’ve been here since I left college. I like working here.'
        },
        {
          name:'Patti:',
          speech:'Really? I’ve only been here for three years, and I’m already tired of doing the same thing every day. I’m afraid of getting really bored'
        },
        {
          name:'Jeff:',
          speech:'Oh, come on! It’s not that bad. You’ll do the same thing there every day.'
        },
        {
          name:'Patti:',
          speech:'Yes, but the salaries are good.'
        },
        {
          name:'Jeff:',
          speech:'I’m not interested in making more money. I have enough now.'
        },
        {
          name:'Patti:',
          speech:'I can never have enough. Of course, you live at home with your parents.'
        },
        {
          name:'Jeff:',
          speech:'I like living with my parents. What’s wrong with that?'
        },
        {
          name:'Patti:',
          speech:'Nothing. But I like being independent. I like traveling and I enjoy meeting new people. I’m going to apply for the job.'
        },
        {
          name:'Jeff:',
          speech:'Well, good luck.'
        },
        ],

        translations:[
        {
          name:'Patti:',
          speech:'Jeff, 뉴욕 센티넬에서 이 광고 봤어요?'
        },
        {
          name:'Jeff:',
          speech:'네, 봤어요. 하지만 새 직장을 구하는 데는 관심이 없어요. 대학을 졸업한 이후로 계속 여기에 있었어요. 저는 여기서 일하는 게 좋아요.'
        },
        {
          name:'Patti:',
          speech:'그래요? 여기 온 지 3년밖에 안 되지만 매일 똑같은 일에 이미 질렸어요. 저는 정말 지루해지는 게 두려워요.'
        },
        {
          name:'Jeff:',
          speech:'아, 어서요! 그렇게 나쁘진 않아요. 매일 거기서 똑같은 일을 하게 될 거예요.'
        },
        {
          name:'Patti:',
          speech:'네, 하지만 월급은 괜찮습니다.'
        },
        {
          name:'Jeff:',
          speech:'저는 더 많은 돈을 버는 것에 관심이 없어요. 이제 충분해요.'
        },
        {
          name:'Patti:',
          speech:'저는 절대 충분치 않아요. 물론, 여러분은 부모님과 함께 집에서 삽니다.'
        },
        {
          name:'Jeff:',
          speech:'저는 부모님과 함께 사는 것을 좋아해요. 그게 뭐가 문제죠?'
        },
        {
          name:'Patti:',
          speech:'아무것도 아닙니다. 하지만 저는 독립적이 되는 것을 좋아합니다. 저는 여행을 좋아하고 새로운 사람들을 만나는 것을 즐깁니다. 저는 그 직업에 지원할 거에요.'
        },
        {
          name:'Jeff:',
          speech:'음, 행운을 빌어요.'
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
