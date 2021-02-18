<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/grandfather-boy-fishing-together_176532-10740.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Times change
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Times change</li><br />

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
          Mr. Brandy has been around for a long time and has opinions about everything. He likes to talk about how things have changed since he was a young man. Do you agree with his comments? Why or why not?
        </p>
        <br />
        <ol style="margin: 12px;">
          <li>
            "Life is much easier nowadays. Machines do all the work." <br />
          </li>
          <li>
            "People are less friendly nowadays. Most people don't even know their neighbors." <br />
          </li>
          <li>
            "People are healthier nowadays. They eat better and live longer. <br />
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
                      back then : 그 때에는 <br />
                    </li>
                    <li>
                      When I was your age : 내가 너 나이였을 때<br />
                    </li>
                    <li>
                      cheek to cheek : 뺨을 맞대고
                    </li>
                    <li>
                      one of 최상급 : 가장 ~중 하나
                    </li>
                    <li>
                      times change : 시간이 지나다
                    </li>
                    <li>
                      problem with : ~으로 골치를 썩다
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
          speech:'Mr. Brady, can I ask you something?'
        },
        {
          name:'B:',
          speech:'Sure, kid.'
        },
        {
          name:'A:',
          speech:'What was it like when you were young?'
        },
        {
          name:'B:',
          speech:'You really want to know?'
        },
        {
          name:'A:',
          speech:'Yes.'
        },
        {
          name:'B:',
          speech:'Well, of course, everything was different back then. Music, clothes, entertainment…'
        },
        {
          name:'A:',
          speech:'What was the music like?'
        },
        {
          name:'B:',
          speech:'It was terrific. When I was your age, we listened to big band music by Glenn Miller and Duke Ellington. You have your rock ’n’ roll which is OK, but the music we had was much more romantic. We liked to dance cheek-to-cheek.'
        },
        {
          name:'A:',
          speech:'Were you a good dancer, Mr. Brady?'
        },
        {
          name:'B:',
          speech:'I don’t like to brag, kid, but I was one of the best. All the girls loved to dance with me. I was the king of the Starlight Ballroom.'
        },
        {
          name:'A:',
          speech:'The Starlight Ballroom? Where’s that?'
        },
        {
          name:'B:',
          speech:'They closed it down twenty years ago.'
        },
        {
          name:'A:',
          speech:'Oh, that was dumb.'
        },
        {
          name:'B:',
          speech:'That’s life. Times change.'
        },
        {
          name:'A:',
          speech:'Do you think times were better then or now?'
        },
        {
          name:'B:',
          speech:'Well, when I was young, life was slower and less complicated. We had fewer problems with noise, pollution and crime. But some things are better now, like medicine and transportation.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'Brady 씨, 뭐 좀 물어봐도 될까요?'
        },
        {
          name:'B:',
          speech:'물론, 꼬마야.'
        },
        {
          name:'A:',
          speech:'어렸을 때 어땠어요?'
        },
        {
          name:'B:',
          speech:'정말 알고 싶어?'
        },
        {
          name:'A:',
          speech:'네.'
        },
        {
          name:'B:',
          speech:'음, 물론 그때는 모든 게 달랐어. 음악, 옷, 오락 같은 거.'
        },
        {
          name:'A:',
          speech:'음악은 어땠어요?'
        },
        {
          name:'B:',
          speech:'정말 좋았어.내가 너 나이였을 때, 우리는 글렌 밀러와 듀크 엘링턴의 빅 밴드 음악을 들었어. 록앤롤은 괜찮지만, 우리가 가지고 있는 음악은 훨씬 더 로맨틱했어. 우리는 건방지게 춤추는 것을 좋아했어.'
        },
        {
          name:'A:',
          speech:'Brady 씨, 춤 잘 추셨어요?'
        },
        {
          name:'B:',
          speech:'자랑하고 싶진 않지만, 최고 중 하나였어. 모든 소녀들이 나와 함께 춤추는 것을 좋아했어.  스타라이트 볼룸의 왕이었어.'
        },
        {
          name:'A:',
          speech:'스타라이트 볼룸요? 거기가 어디죠?'
        },
        {
          name:'B:',
          speech:'20년 전에 문을 닫았어.'
        },
        {
          name:'A:',
          speech:'아, 그건 바보 같았어요.'
        },
        {
          name:'B:',
          speech:'그게 인생이야. 시대가 바껴.'
        },
        {
          name:'A:',
          speech:'그때가 좋았다고 생각하세요, 아니면 지금이라고 생각하세요?'
        },
        {
          name:'B:',
          speech:'음, 어렸을 때, 삶은 더 느리고 덜 복잡했어. 우리는 소음, 오염, 범죄에 대한 문제가 적었어. 하지만 지금은 더 나아진 것도 있어. 약이나 교통수단과 같은 것들.'
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
