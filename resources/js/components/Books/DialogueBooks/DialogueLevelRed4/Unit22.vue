<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/parking_1127-2914.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Where's it gone?
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Where's it gone?</li><br />

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
          Ex) Anna has a toothache. She isn't here. > She's gone to the dentist.<br />
        </p>

        <ol style="margin: 12px;">
          <li>
            John needs some money. He isn't here.  >   <u> &emsp; &emsp; &emsp; </u><br />
          </li>
          <li>
            Kelly broke her arm. She isn't here.  >   <u> &emsp; &emsp; &emsp; </u><br />
          </li>
          <li>
            Andrea forgot to get eggs. She isn't here.  >   <u> &emsp; &emsp; &emsp; </u><br />
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
                      현재완료의 용법 : 경험 -과거에서 지금까지의 경험을 물어볼 때(~한 적이 있다),<br />
                                  계속 - 과거에 일어났던 일이 현재까지 계속 되고 있을 때,<br />
                                  결과 - 과거의 일이 원인이 되어 그 결과가 현재에도 영향을 미칠 때,<br />
                                  완료 - 과거에 시작한 일을 현재 막 끝낸 것을 나타낼 때,<br />
                    </li>
                    <li>
                      현재완료의 의문문 : Have(has) + 주어 + 과거분사..?<br />
                    </li>
                    <li>
                      현재완료의 부정문 : 주어 + have(has) + not(never) + 과거분사...<br />
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
          name:'Kelly:',
          speech:'OK. Which way is the car?'
        },
        {
          name:'Mark:',
          speech:'It’s in space 34. It’s this way.'
        },
        {
          name:'Kelly:',
          speech:'I can’t see it.'
        },
        {
          name:'Mark:',
          speech:'No, Kelly. It’s gone!'
        },
        {
          name:'Kelly:',
          speech:'Are you sure?'
        },
        {
          name:'Mark:',
          speech:'Yes. It was in space 34. It isn’t there now. It’s gone, Kelly. It really has gone. This is terrible! It’s only two months old.'
        },
        {
          name:'Kelly:',
          speech:'Come on! Where’s it gone? This is a high-security parking garage. You can’t get out without the ticket, and you have the ticket.'
        },
        {
          name:'Mark:',
          speech:'But space 34 is empty — and it’s the right number. I wrote it on the ticket.'
        },
        {
          name:'Kelly:',
          speech:'Let me see. Oh, Mark. It hasn’t gone! We’re on the wrong floor! Look, this is floor C. The car’s on floor D.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Paul:',
          speech:'Hey, Bill, can you lend me $10?'
        },
        {
          name:'Bill:',
          speech:'Sorry, I can’t. I haven’t been to the bank today.'
        },
        {
          name:'Paul:',
          speech:'Oh, I haven’t been there either, and I need some money. We could go now.'
        },
        {
          name:'Bill:',
          speech:'No, the bank’s closed. It’s too late. Why don’t you ask Pete?'
        },
        {
          name:'Paul:',
          speech:'Has he been to the bank?'
        },
        {
          name:'Bill:',
          speech:'Yes, he has. He always goes to the bank on Mondays.'
        },
        ],

        translations:[
        {
          name:'Kelly:',
          speech:'알았어요. 차는 어느 쪽입니까?'
        },
        {
          name:'Mark:',
          speech:'34번 자리에 있어요. 이쪽입니다.'
        },
        {
          name:'Kelly:',
          speech:'안 보여요.'
        },
        {
          name:'Mark:',
          speech:'아니요, Kelly. 사라졌어요!'
        },
        {
          name:'Kelly:',
          speech:'확실해요?'
        },
        {
          name:'Mark:',
          speech:'그렇습니다. 그것은 34번 자리에 있었습니다. 그것은 지금 그곳에 없습니다. 사라졌어요, Kelly 정말 사라졌어요. 끔찍해요! 산 지 두 달밖에 안 됐어요.'
        },
        {
          name:'Kelly:',
          speech:'어서요! 어디로 갔죠? 여기는 보안이 철저한 주차장이에요. 표 없이는 나갈 수 없고, 표도 있습니다.'
        },
        {
          name:'Mark:',
          speech:'하지만 34는 비어 있습니다. 그리고 그것은 올바른 숫자입니다. 표에 적어놨어요.'
        },
        {
          name:'Kelly:',
          speech:'어디 보죠. 오, Mark요. 아직 안 갔어요! 우리는 잘못된 층에 있어요! 보세요 여기는 C층입니다. 차는 D층에 있어요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'Paul:',
          speech:'Bill, 10달러만 Bill려줄 수 있어요?'
        },
        {
          name:'Bill:',
          speech:'죄송해요, 전 못해요. 저는 오늘 은행에 가지 않았어요.'
        },
        {
          name:'Paul:',
          speech:'저도 거기 가보지 않았는데, 돈이 좀 필요해요. 지금 갈 수 있어요.'
        },
        {
          name:'Bill:',
          speech:'아니요, 은행은 문을 닫았어요. 너무 늦었어요. Pete에게 물어보지 그래요?'
        },
        {
          name:'Paul:',
          speech:'그는 은행에 가본 적이 있나요?'
        },
        {
          name:'Bill:',
          speech:'네. 그는 월요일에 항상 은행에 갑니다. '
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
