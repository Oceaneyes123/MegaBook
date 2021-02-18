<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/wave-space-noguchi-astronaut-soichi-travel_121-67710.jpg" class="cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 class="upper-header-DBG3">Return from space
      </h1>
    </v-layout>
  </v-img>

  <hr class="top-line-DBG3">
  <h3 class="lower-header-DBG3">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

    <li style="list-style-type: none;">Return from space</li><br />

    <p>
      Phil Strongarm, the astronaut, is talking about his journey to the moon.<br />
      Opel Winford, the TV personality, is interviewing Phil. <br />
    </p>

    <table style = "border-collapse: collapse;">
    
      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table>

      <div class="line-DBG3">
      </div>
      <h3 class = "border-DBG3 white--text">Exercise</h3>
        <div style="padding : 16px;">

        <p>
          <u>Answer the questions</u><br />
          (질문에 답하시오.)
        </p>

        <ol style="margin: 12px;">
          <li>
            Who’s Phil Strongarm? <br />
              Phil Strongarm은 누구입니까? <br />
          </li>
          <li>
            Was his trip comfortable or uncomfortable?<br />
              그의 여행은 편안했습니까 아니면 불편했습니까?<br />
          </li>
          <li>
            What did he eat? <br />
              그는 무엇을 먹었습니까?<br />
          </li>
        </ol>
        <br />
        <p>
          Free response:<br />
           Would you like to go to the moon? <br />
           What did you have for lunch yesterday?<br />
           How was the weather yesterday?


        </p>



      </div>

      <div class="line-DBG3">
      </div>
      <h3 class = "border-DBG3 white--text">Translation</h3>
      <div style="padding : 16px;">
        <p>
          우주 비행사 Phil Strongarm은 그의 달여행에 대해서 말하고 있습니다.<br />
          TV 인기배우 Opel Winford가 Phil을 인터뷰하고 있습니다.<br />
        </p>

        <table style = "border-collapse: collapse;">

          <tr v-for="translation in translations"  :key="translation">
            <td class = "uppertable" >{{translation.name}}</td>
            <td class = "lowertable" >{{translation.speech}}</td>
          </tr>
  
        </table>

        
</div>
        <div class="line-DBG3">
        </div>
        <h3 class = "border-DBG3 white--text">Self Study</h3>
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
                      have – had ( 과거형 )  / we didn't have ( 과거형부정 ) / did you have? ( 과거형 의문문 )  / <br />
                        what did you have? ( 의문사가 있는 과거형의 의문문 ) <br />
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
          name:'Opel:',
          speech:'Well, Phil, welcome back to Earth.'
        },
        {
          name:'Phil:',
          speech:'Thanks, ma’am. Uh, Ms. Winford… I mean, Opel.'
        },
        {
          name:'Opel:',
          speech:'Did you have any problems on the trip into space?'
        },
        {
          name:'Phil:',
          speech:'We didn’t have any serious problems, but it certainly wasn’t a picnic.'
        },
        {
          name:'Opel:',
          speech:'What do you mean?'
        },
        {
          name:'Phil:',
          speech:'We didn’t have a bath or shave for two weeks.'
        },
        {
          name:'Opel:',
          speech:'Oh, really?'
        },
        {
          name:'Phil:',
          speech:'Yes. It wasn’t very comfortable.'
        },
        {
          name:'Opel:',
          speech:'What about food? Was that a problem?'
        },
        {
          name:'Phil:',
          speech:'Well, we didn’t have any normal food.'
        },
        {
          name:'Opel:',
          speech:'What did you have?'
        },
        {
          name:'Phil:',
          speech:'We had some food tablets and other kinds of food in tubes.'
        },
        {
          name:'Opel:',
          speech:'Are you going to the moon again, Phil?'
        },
        {
          name:'Phil:',
          speech:'I hope so, um, Opel. It was uncomfortable and difficult… but it was wonderful.'
        },
        ],

        translations:[
        {
          name:'Opel:',
          speech:'우선, Phil, 지구로 돌아오신 것을 환영합니다.'
        },
        {
          name:'Phil:',
          speech:'감사합니다. Winford씨... 그러니까, Opel.'
        },
        {
          name:'Opel:',
          speech:'우주에서 당신의 여행에는 어떤 문제가 있었습니까?'
        },
        {
          name:'Phil:',
          speech:'심각한 문제는 없었습니다. 하지만 그것은 분명 소풍은 아니었습니다.'
        },
        {
          name:'Opel:',
          speech:'무슨 의미입니까?'
        },
        {
          name:'Phil:',
          speech:'우리는 2주 동안 목욕이나 면도를 못했습니다.'
        },
        {
          name:'Opel:',
          speech:'오, 정말입니까?'
        },
        {
          name:'Phil:',
          speech:'네. 그다지 편안하지 않았습니다.'
        },
        {
          name:'Opel:',
          speech:'음식은 어땠습니까? 문제가 있었습니까?'
        },
        {
          name:'Phil:',
          speech:'글쎄요, 우리는 보통 음식을 먹지 못했습니다.'
        },
        {
          name:'Opel:',
          speech:'무엇을 드셨습니까?'
        },
        {
          name:'Phil:',
          speech:'우리는 음식 알약과 통에 담겨져 있는 종류의 음식을 먹었습니다.'
        },
        {
          name:'Opel:',
          speech:'당신은 다시 달에 갈 예정이십니까, Phil?'
        },
        {
          name:'Phil:',
          speech:'그러고 싶습니다 Opel. 불편하고 어려웠지만.. 굉장했습니다.'
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


</style>
