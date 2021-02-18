<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/old-photoalbum-arms-tender-yong-woman_8353-1397.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Pictures from the past
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Pictures from the past</li><br />
      <br />
      <p>
        Josh is visiting his mother. He's with his new girlfriend, Rosa. They’re looking at their family photo album.<br />
      </p>
      <br />
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
          Look at the photos and talk about Josh<br />
          <br />
          What could he do when he was 8 (10, 14, 17) years old?<br />
        </p>

        <v-container grid-list-md text-xs-center>
          <v-layout wrap align-content-center>

            <v-flex xs12 md4 >
              <v-card hover>

                <v-img src="images/kfcmap.gif" />

              </v-card>
            </v-flex>

          </v-layout>
        </v-container>

        <p>
          Free response:<br />
          <br />
          How old were you when you could walk / cook / etc.?<br />
        </p>



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
          Josh 는 그의 어머니를 방문하고 있습니다. 새 여자친구 Rosa와 함께 있어요 그들은 가족 사진첩을 보고 있습니다.<br />
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
                      When : 시간을 나타내는 접속사로 보통 '~할 때'의 뜻이지만 경우에 따라서는 '~할 때마다'의 의미로 쓰이기도 합니다. When절은 문장 앞 뒤 어느 쪽에도 올 수 있습니다.<br />
                    </li>
                    <li>
                      Could : 마음만 먹으면 언제든지 할 수 있었다는 과거의 평상시 능력을 나타낼 때 사용됩니다<br />
                          Ex) Josh could sit up when he was a six month old : Josh는 6개월 되었을 때 설 수 있었다<br />
                              He could talk when he was a year : 그는 한 살 때 말할 수 있었다<br />
                              When he was three he could swim : 그는 세 살 때 수영할 수 있었다<br />
                              I couldn't swim until I was five or six : 내가 다섯 살이나 여섯 살 때까지는 수영할 수 없었다 <br />
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
          name:'Rosa:',
          speech:'That’s a nice picture of Josh, Mrs. Ryan. Did you take it?'
        },
        {
          name:'Mrs. Ryan:',
          speech:'Yes. Photography’s my hobby. I have a lot of pictures of Josh.'
        },
        {
          name:'Rosa:',
          speech:'Oh, really? May I see some?'
        },
        {
          name:'Mrs. Ryan:',
          speech:'Why, yes. There’s an album here.'
        },
        {
          name:'Josh:',
          speech:'Oh, no, Mom! Not the photographs! Please!'
        },
        {
          name:'Rosa:',
          speech:'Shh. I want to see them. Oh, wow!'
        },
        {
          name:'Mrs. Ryan:',
          speech:'Look, Josh could sit up when he was six months old.'
        },
        {
          name:'Rosa:',
          speech:'That’s really cute!'
        },
        {
          name:'Mrs. Ryan:',
          speech:'And he could talk when he was a year... look.'
        },
        {
          name:'Josh:',
          speech:'This is awful. Please, Mom…'
        },
        {
          name:'Mrs. Ryan:',
          speech:'Be quiet, Joshua. When he was three he could swim.'
        },
        {
          name:'Rosa:',
          speech:'Really? I couldn’t swim until I was five or six.'
        },
        {
          name:'Mrs. Ryan:',
          speech:'This is a picture on the beach…'
        },
        {
          name:'Josh:',
          speech:'Mom! I’m not wearing any clothes in that picture!'
        },
        ],

        translations:[
        {
          name:'Rosa:',
          speech:'Josh 의 멋진 사진이군요, Ryan 부인. 그것을 가져가셨나요?'
        },
        {
          name:'Mrs. Ryan:',
          speech:'응. 사진은 내 취미야. 나는 Josh 의 사진을 많이 가지고 있어.'
        },
        {
          name:'Rosa:',
          speech:'아, 그래요? 좀 볼 수 있을까요?'
        },
        {
          name:'Mrs. Ryan:',
          speech:'응. 여기 앨범이 있어.'
        },
        {
          name:'Josh:',
          speech:'엄마! 사진은 안돼요! 제발!'
        },
        {
          name:'Rosa:',
          speech:'쉿. 나는 그들을 보고싶어. 오, 와우!'
        },
        {
          name:'Mrs. Ryan:',
          speech:'봐봐, Josh 는 6개월 때 일어설 수 있었어'
        },
        {
          name:'Rosa:',
          speech:'정말 귀엽네요!'
        },
        {
          name:'Mrs. Ryan:',
          speech:'그리고 그는 1살 때 말할 수 있었어... 봐'
        },
        {
          name:'Josh:',
          speech:'이건 정말 끔찍해요. 제발요, 엄마…'
        },
        {
          name:'Mrs. Ryan:',
          speech:'조용히 해, 조슈아. 그는 세 살 때 수영을 할 수 있었어.'
        },
        {
          name:'Rosa:',
          speech:'그래요? 저는 대여섯 살이 될 때까지 수영을 할 수 없었어요.'
        },
        {
          name:'Mrs. Ryan:',
          speech:'이것은 해변에 있는 사진이야.'
        },
        {
          name:'Josh:',
          speech:'엄마! 저 사진 속 옷은 하나도 안 입었어요!'
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
