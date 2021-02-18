<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/spacecraft_1048-4457.jpg" class="cover-photo">

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
        padding-bottom: 10px;">UFO
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">UFO</li><br />

      <br />
      <p>
        Dick and Janet were driving along a quiet country road in Ohio. They were on their way to Cincinnati. It was almost midnight.<br />
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
          <u>Combine the sentences</u><br />
          Ex) What is it? (I don’t know.)   >   I don’t know what it is.
        </p>
        <br />
        <ol style="margin: 12px;">
          <li>
            What was it? (They don’t know.)   >
          </li>
          <li>
            Why wasn’t the car working? (They wondered.)  >
          </li>
          <li>
            What happened to the car? (He doesn’t know.)   >
          </li>
          <li>
            Is the service station open? ( She doesn’t know.)  >
          </li>
        </ol>

        <br />
        <p>
          Free response:<br />
            Do you believe in UFO? Have you ever seen any?<br />
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
          Dick 과 Janet 은 오하이오의 조용한 시골길을 따라 운전하고 있었습니다. 그들은 신시내티로 가는 길이었어요. 거의 자정이 다 된 시간이었어요.<br />
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
                      간접의문문 : <br />
                          I don't know what it is. (나는 그것이 무엇인지 모르겠다) : I don't know. + What is it? <br />
                          I don't know if it's open. (나는 그것이 열렸는지 모르겠다) : I don't know. + Is it open?<br />
                    </li>
                    <li>
                      on one's way : ~ 가는 도중에
                    </li>
                    <li>
                      look over : 위를 보다
                    </li>
                    <li>
                      the engine just died : 엔진이 방금 나갔다
                    </li>
                    <li>
                      "What has happened to it?" 어떻게 된 거야? (무슨 일이야?) 
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
          name:'Janet',
          speech:'Dick, look over there. There’s something in the sky. What is it?'
        },
        {
          name:'Dick:',
          speech:'I don’t know what it is. It’s probably a plane.'
        },
        {
          name:'Janet',
          speech:'I don’t think so. It’s too big — and too bright.'
        },
        {
          name:'Dick:',
          speech:'You’ve seen too many movies, Janet… Oh, no!'
        },
        {
          name:'Janet',
          speech:'What’s the matter?'
        },
        {
          name:'Dick:',
          speech:'The engine just died.'
        },
        {
          name:'Janet',
          speech:'What’s happened to it?'
        },
        {
          name:'Dick:',
          speech:'Well, I don’t know what happened. We’ll have to find a service station.'
        },
        {
          name:'Janet',
          speech:'There’s one in the next town.'
        },
        {
          name:'Dick:',
          speech:'Great, but I don’t know if it’s open. It’s really late.'
        },
        ],

        translations:[
        {
          name:'Janet',
          speech:'Dick , 저기를 보세요. 하늘에 뭔가 있어요. 뭔데요?'
        },
        {
          name:'Dick:',
          speech:'뭔지 모르겠어요. 아마 비행기일 거예요..'
        },
        {
          name:'Janet',
          speech:'난 그렇게 생각하지 않아요. 그것은 너무 크고 너무 밝습니다.'
        },
        {
          name:'Dick:',
          speech:'당신은 영화를 너무 많이 봤어요, Janet . 오, 안돼요!'
        },
        {
          name:'Janet',
          speech:'무슨 일이에요?'
        },
        {
          name:'Dick:',
          speech:'엔진이 방금 죽었어요.'
        },
        {
          name:'Janet',
          speech:'어떻게 된 거죠?'
        },
        {
          name:'Dick:',
          speech:'글쎄, 무슨 일이 있었는지 모르겠어요. 서비스 센터를 찾아야겠어요.'
        },
        {
          name:'Janet',
          speech:'옆 동네에 하나 있어요.'
        },
        {
          name:'Dick:',
          speech:'좋아요, 하지만 열려있는지 모르겠어요. 정말 늦었어요'
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
