<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/new-orleans-saint-louis-cathedral_19-108940.jpg" class="cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 class="upper-header-DBB5">Trip to New Orleans
      </h1>
    </v-layout>
  </v-img>

  <hr class="top-line-DBB5">
  <h3 class="lower-header-DBB5">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

    <li style="list-style-type: none;">Trip to New Orleans</li><br />

    <table style = "border-collapse: collapse;">
    
      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table>

      <div class="line-DBB5">
      </div>
      <h3 class = "border-DBB5 white--text">Exercise</h3>
        <div style="padding : 16px;">

        <p>
          <u>Complete the conversations using the present perfect</u><br />
        </p>

        <ol style="margin: 12px;">
          <li>
            <br />
            A: Have you <u> &emsp; &emsp; &emsp; </u> much exercise this week? ( do )<br />
            B: Yes, I <u> &emsp; &emsp; &emsp; </u> already <u> &emsp; &emsp; &emsp; </u> to aerobics class four times. ( be )
          </li>
          <li>
            <br />
            A: How many movies <u> &emsp; &emsp; &emsp; </u> you <u> &emsp; &emsp; &emsp; </u> to this month? ( be )
            B: Actually, I <u> &emsp; &emsp; &emsp; </u>    <u> &emsp; &emsp; &emsp; </u> any yet. ( see )
          </li>
        </ol>

      </div>

      <div class="line-DBB5">
      </div>
      <h3 class = "border-DBB5 white--text">Translation</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr v-for="translation in translations"  :key="translation">
            <td class = "uppertable" >{{translation.name}}</td>
            <td class = "lowertable" >{{translation.speech}}</td>
          </tr>
  
        </table>

        
</div>
        <div class="line-DBB5">
        </div>
        <h3 class = "border-DBB5 white--text">Self Study</h3>
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
                      to부정사의 부사적 용법 : to부정사가 부사처럼 쓰여 동사, 형용사, 다른 부사등을 수식합니다.<br />
                      감정을 나타내는 형용사 뒤의 to부정사는 감정의 원인을 나타내며 ~해서라고 해석합니다.<br />
                      (감정을 나타내는 형용사 : happy, glad, sad, sorry, pleased, surprised, excited)<br />
                      Ex) I'm really excited to be here : 여기에 있어서 정말 흥분된다<br />
                    </li>
                    <li>
                      수여동사가 있는 문장의 순서 : 주어+수여동사+간접목적어+직접목적어<br />
                      (수여동사 : give, buy, show, send, make...)<br />
                      Ex) I can't wait to show you the city (show:수여동사, you:간접목적어, the city:직접목적어)<br />
                    </li>
                    <li>
                      a few days : 며칠
                    </li>
                    <li>
                      that's how : 그것이 ~한 방법이다 / that's why : 그것이 ~한 이유이다
                    </li>
                    <li>
                      take it easy : 느긋하게 하다, 쉬다
                    </li>
                    <li>
                      my feet are killing me : 발이 아파 죽겠다
                    </li>
                    <li>
                      "You're kidding!" : 장난이지?, 날 놀리지마
                    </li>
                    <li>
                      how many years have you lived in..? : ~에 몇 년 동안 살고 있니? (~온지 얼마나 되었니?) 
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
          speech:'It’s great to see you, Todd. Have you been to New Orleans long?'
        },
        {
          name:'B:',
          speech:'Just a few days. I’m really excited to be here.'
        },
        {
          name:'A:',
          speech:'I can’t wait to show you the city. Have you been to a jazz club yet?'
        },
        {
          name:'B:',
          speech:'Yeah, I’ve already been to one.'
        },
        {
          name:'A:',
          speech:'Oh. Well, how about a riverboat tour?'
        },
        {
          name:'B:',
          speech:'Uh, I’ve already done that, too.'
        },
        {
          name:'A:',
          speech:'Have you ridden in a streetcar? They’re a lot of fun.'
        },
        {
          name:'B:',
          speech:'Actually, that’s how I got here today.'
        },
        {
          name:'A:',
          speech:'Well, is there anything you want to do?'
        },
        {
          name:'B:',
          speech:'You know, I really just want to take it easy. My feet are killing me!'
        },
        {
          name:'A:',
          speech:'So let’s just stay here and relax. I know you’re tired.'
        },
        {
          name:'B:',
          speech:'Thanks, Jan. But we can plan something for tomorrow.'
        },
        {
          name:'A:',
          speech:'Great! Have you been to the zoo?'
        },
        {
          name:'B:',
          speech:'No, I haven’t. But I’ve heard it’s good. Let’s go there in the afternoon.'
        },
        {
          name:'A:',
          speech:'OK.'
        },
        {
          name:'B:',
          speech:'Say, have you been to the French market? I’d love to go there, too.'
        },
        {
          name:'A:',
          speech:'Actually, I’ve never been there.'
        },
        {
          name:'B:',
          speech:'You’re kidding! And how many years have you lived in New Orleans? We have to go there.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'만나서 반가워, Todd. New Orleans에는 얼마나 가봤니?'
        },
        {
          name:'B:',
          speech:'며칠만. 여기 와서 정말 신난다'
        },
        {
          name:'A:',
          speech:'빨리 도시를 보여 주고 싶어. 재즈 클럽에 가본 적 있니?'
        },
        {
          name:'B:',
          speech:'응, 벌써 한 군데 가봤어.'
        },
        {
          name:'A:',
          speech:'아, 그럼, 리버 보트 투어는 어때?'
        },
        {
          name:'B:',
          speech:'어, 나도 이미 그렇게 했어.'
        },
        {
          name:'A:',
          speech:'전차를 타 봤어? 매우 재밌어.'
        },
        {
          name:'B:',
          speech:'사실, 오늘 그렇게 왔어.'
        },
        {
          name:'A:',
          speech:'음, 뭐 하고 싶은 거 있어?'
        },
        {
          name:'B:',
          speech:'있잖아, 난 그냥 좀 진정하고 싶어. 발이 아파 죽겠어!'
        },
        {
          name:'A:',
          speech:'그럼 그냥 여기 있으면서 쉬자. 피곤한 거 알아.'
        },
        {
          name:'B:',
          speech:'고마워, Jan. 하지만 우리는 내일을 위해 무언가를 계획할 수 있어.'
        },
        {
          name:'A:',
          speech:'좋아! 동물원에 가본적 있니?'
        },
        {
          name:'B:',
          speech:'아니, 못 봤어. 하지만 좋다고 들었어. 오후에 그곳에 가자.'
        },
        {
          name:'A:',
          speech:'알았어'
        },
        {
          name:'B:',
          speech:'프랑스 시장에 가본 적 있어? 나도 그곳에 가고 싶어.'
        },
        {
          name:'A:',
          speech:'사실, 한번도 가 본 적이 없어.'
        },
        {
          name:'B:',
          speech:'농담하는 거야! 그리고 뉴올리언스에서 몇 년이나 살았니? 우리는 그곳에 가야 해.'
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
