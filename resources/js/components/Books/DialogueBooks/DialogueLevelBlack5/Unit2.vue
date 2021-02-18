<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/various-electronic-gadgets-wooden-background_23-2147797027.jpg" class="cover-photo">

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
        padding-bottom: 10px;">An electronic world?
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

    <li style="list-style-type: none;">An electronic world?</li><br />


    <table style = "border-collapse: collapse;">
    
      <tr v-for="dialog in dialogs"  :key="dialog">
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

        <ol style="margin: 12px;">
          <li>
            Which of these things have you used this week?<br />
              <br />
                a. a camera<br />
                b. a mobile phone<br />
                c. a computer<br />
                d. an MP3 player<br />
                e. a microwave oven<br />
          </li>
          <li>
            How many of the things above do you use every day?
          </li>
          <li>
            Choose one item from question #1 and answer:<br />
            <br />
                - Who bought it?<br />
                - How old is it?<br />
                - What brand is it?<br />
                - What do you use it for?<br />
                - Does it save your time?<br />
                - Does it save your money?<br />
                - Do you really need it?<br />
                - Is it important in your life?<br />
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

          <tr v-for="translation in translations"  :key="translation">
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
                      for와 during : <br />
                          for - ~동안, for 뒤에는 구체적인 숫자나 기간 (시간, 날짜, 년 등)이 옵니다. How long~?으로 묻는 말에 응답할 때 사용됩니다. <br />
                          during - ~동안, 행사나 사건등의 앞에 쓰입니다. When~?으로 묻는 말에 응답할 때 사용됩니다.<br />
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
          name:'Flight attendant:',
          speech:'Pardon me, sir. Is everything here yours?'
        },
        {
          name:'Mr. Gabriel:',
          speech:'Yes, that’s right.'
        },
        {
          name:'Flight attendant:',
          speech:'I’m sorry, sir. You can’t use any electronic equipment during takeoff and landing.'
        },
        {
          name:'Mr. Gabriel:',
          speech:'Why not?'
        },
        {
          name:'Flight attendant:',
          speech:'It’s an airline regulation, sir. You can use the CD player during the flight, but I’m afraid you can’t use the laptop computer or the portable phone…or the portable TV.'
        },
        {
          name:'Mr. Gabriel:',
          speech:'But I have to use my computer. I need it!'
        },
        {
          name:'Flight attendant:',
          speech:'I’m very sorry.'
        },
        {
          name:'Mr. Gabriel:',
          speech:'But I can’t live without it! What am I going to do for two hours?'
        },
        {
          name:'Flight attendant:',
          speech:'You can read, sir.'
        },
        {
          name:'Mr. Gabriel:',
          speech:'Read? But I don’t have any books.'
        },
        {
          name:'Flight attendant:',
          speech:'I’ll get you a magazine, sir'
        },
        ],

        translations:[
        {
          name:'승무원:',
          speech:'죄송합니다, 손님. 여기 있는 건 다 당신 건가요?'
        },
        {
          name:'Gabriel 씨:',
          speech:'네, 맞습니다.'
        },
        {
          name:'승무원:',
          speech:'죄송합니다. 이륙과 착륙 중에는 어떤 전자 장비도 사용할 수 없습니다.'
        },
        {
          name:'Gabriel 씨:',
          speech:'왜 안되죠?'
        },
        {
          name:'승무원:',
          speech:'항공사 규정입니다. CD 플레이어는 비행 중에 사용할 수 있지만 노트북 컴퓨터나 휴대용 전화기, 휴대용 TV는 사용할 수 없습니다.'
        },
        {
          name:'Gabriel 씨:',
          speech:'하지만 저는 컴퓨터를 사용해야 합니다. 그게 필요해요!'
        },
        {
          name:'승무원:',
          speech:'대단히 죄송합니다.'
        },
        {
          name:'Gabriel 씨:',
          speech:'하지만 그것 없이는 살 수 없어요! 두 시간 동안 저는 무엇을 할 건가요?'
        },
        {
          name:'승무원:',
          speech:'읽으실 수 있습니다'
        },
        {
          name:'Gabriel 씨:',
          speech:'읽으라구요? 하지만 저는 책이 하나도 없어요.'
        },
        {
          name:'승무원:',
          speech:'잡지를 갖다 드리겠습니다, 손님.'
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
