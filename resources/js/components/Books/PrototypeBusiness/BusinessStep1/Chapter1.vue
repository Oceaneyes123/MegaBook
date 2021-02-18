<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/VhjZo/MADyQ1VhjZo/1/s2/canva-woman-smiling-shaking-hands-MADyQ1VhjZo.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 class="upper-border-BS1">Meeting People
      </h1>
    </v-layout>
  </v-img>

 <div class="top-line-BS1">
  </div>
  <h3  class = "lower-header-BS1 white--text" >Today's topic</h3>
  <div style = "padding : 16px;">


    <table style = "border-collapse: collapse;" :key="dialog">
      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>
    
  </table>


  <div class="line-BS1">
    </div>
    <h3 class = "border-BS1 white--text">Translation</h3>
    <div style="padding : 16px;">

    <table style = "border-collapse: collapse;">

      <tr v-for="translation in translations" :key="translation">
        <td class = "uppertable" >{{translation.name}}</td>
        <td class = "lowertable" >{{translation.speech}}</td>
      </tr>
    
    </table>  
   
    
  </div>

      <v-container grid-list-md text-xs-center>
        <v-layout wrap align-content-center>

          <v-flex xs6 md2>
            <v-expand-transition>
            <v-card hover>

              <v-card-media height="400px" src="https://image.freepik.com/free-photo/african-american-smiling-businessman-suit-glasses-looking-camera_1163-3902.jpg">
                <v-card-text class = "profile-card-BS1"><font color = "white">
                  Paul Sampson<br />
                  -ZY Communications
                </font></v-card-text>
              </v-card-media>


            </v-card>
          </v-expand-transition>
          </v-flex>

          <v-flex xs6 md2>
            <v-expand-transition>
            <v-card hover>

              <v-card-media height="400px" src="https://image.freepik.com/free-photo/happy-successful-woman-posing-with-folded-arms_1262-21095.jpg">
                <v-card-text class = "profile-card-BS1"><font color = "white">
                  Lara Kay<br />
                  -ZY Holdings
                </font></v-card-text>
              </v-card-media>


            </v-card>
          </v-expand-transition>
          </v-flex>

          <v-flex xs6 md2>
            <v-expand-transition>
            <v-card hover>

              <v-card-media height="400px" src="https://image.freepik.com/free-photo/confident-businessman-looking-camera_23-2148112837.jpg">
                <v-card-text class = "profile-card-BS1"><font color = "white">
                  Sam Pick<br />
                  -ZY Holdings
                </font></v-card-text>
              </v-card-media>


            </v-card>
          </v-expand-transition>
          </v-flex>

          <v-flex xs6 md2>
            <v-expand-transition>
            <v-card hover>

              <v-card-media height="400px" src="https://image.freepik.com/free-photo/elegant-businesswoman-holding-clipboard_1098-3344.jpg">
                <v-card-text class = "profile-card-BS1"><font color = "white">
                  Anne Pol<br />
                  -ZY Design
                </font></v-card-text>
              </v-card-media>


            </v-card>
          </v-expand-transition>
          </v-flex>

          <v-flex xs6 md2>
            <v-expand-transition>
            <v-card hover>

              <v-card-media height="400px" src="https://image.freepik.com/free-photo/successful-indian-businessman-with-digital-tablet_1262-3325.jpg">
                <v-card-text class = "profile-card-BS1"><font color = "white">
                  David Tarn<br />
                  -ZY Design
                </font></v-card-text>
              </v-card-media>


            </v-card>
          </v-expand-transition>
          </v-flex>

        </v-layout>
      </v-container>






      <div class = "line-BS1">
      </div>
      <h3 class = "border-BS1 white--text">Exercise</h3>
      <div style="padding : 16px;">

        <p>
          Fill in the gaps with the correct form of be
        </p>

        <ol style="margin: 12px;">
          <li>
            I’m Paul Reed and this is Julia Bell. ( &emsp; &emsp; ) from Zap Productions.
          </li>
          <li>
            This is Diana Edison. ( &emsp; &emsp; ) from B-Line.
          </li>
          <li>
            I’m David Clark. ( &emsp; &emsp; ) from Safeguard.
          </li>
        </ol>

      </div>

      <div class = "line-BS1">
      </div>
      <h3 class = "border-BS1 white--text">Self Study</h3>
      <div style="padding : 16px;">


          <p>
            Notes
          </p>

        <p>

          <v-container grid-list-md text-xs-left>
            <v-layout row wrap>


              <v-flex xs12>
                <v-card light color="#9197A6">
                  <v-card-text class="px-10">
                    <p>
                      be 동사
                    </p>
                    <p>
                      I am (I’m) ~<br />
                      He is (He’s) ~<br />
                      We are (We’re) ~<br />
                      You are (You’re) ~<br />
                      She is (She’s) ~<br />
                      They are (They’re) ~<br />
                    </p>
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
          name:'Joe:',
          speech:'Hello everyone. This is Claire Martin. She’s from IBM. Claire, this is Paul Sampson. He’s from ZY Communications.'
        },
        {
          name:'Paul:',
          speech:'Hello Claire.'
        },
        {
          name:'Joe:',
          speech:'And this is Anne Pol and David Tarn. They’re from ZY Design.'
        },
        {
          name:'David:',
          speech:'Nice to meet you.'
        },
        {
          name:'Anne:',
          speech:'Hello'
        },
        {
          name:'Sam:',
          speech:'And I’m Sam Pick and this is Lara Kay. We’re from ZY Holdings. So, You’re from New York, Claire?'
        },
        {
          name:'Claire:',
          speech:'Yes. Nice to meet you, everyone.'
        },

        ],

        translations:[
        {
          name:'조:',
          speech:"여러분 안녕하세요. 이쪽은 클레어 마틴입니다. 그녀는 IBM 출신입니다. 클레어, 이쪽은 폴 샘슨이에요 ZY Communications에서 왔어요."
        },
        {
          name:'폴:',
          speech:"안녕하세요 클레어."
        },
        {
          name:'조:',
          speech:"그리고 이쪽은 앤 폴과 데이비드 타른입니다. ZY Design에서 나왔습니다."
        },
        {
          name:'데이비드:',
          speech:"만나서 반가워요."
        },
        {
          name:'앤:',
          speech:"안녕하세요."
        },
        {
          name:'샘:',
          speech:"그리고 저는 샘 픽이고 이쪽은 라라 케이입니다. 저희는 ZY 홀딩스 출신입니다. 뉴욕 출신이에요, 클레어?"
        },
        {
          name:'클레어:',
          speech:"네. 만나서 반가워요, 여러분."
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
