<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/pocket-watch-box-with-sequins_23-2147992709.jpg" class="cover-photo">

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
        padding-bottom: 10px;">How long ago?
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">How long ago?</li><br />
      
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
            How long ago did you wake up?<br />
          </li>
          <li>
            How long ago did you read newspapers?<br />
          </li>
          <li>
            How long ago did you eat?<br />
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
                      ago : '(지금으로부터)~전에'라는 의미로 two years ago, a long time ago 등과 같이 기간을 나타내는 어구와 함께 사용됩니다. 과거를 나타내므로 원칙상 '과거시제'와 함께 쓰입니다.<br />
                      ago 앞에 기간을 나타내는 어구가 있어 과거의 특정시간이 되므로 현재완료와 쓰일 수 없습니다.<br />
                    </li>
                    <li>
                      ... a book called Modern Banking : Modern Banking이라고 불리우는 책이고 a book과 called사이에 which is가 생략되었습니다. <br />
                    </li>
                    <li>
                      수여동사 : 간접목적어와 직접목적어를 갖는 동사이고 형식은<br />
                      주어+수여동사+간접목적어(~에게)+직접목적어(~을)입니다.<br />
                      하지만 간접목적어와 직접목적어의 순서는 바뀔 수 있는데 그럴 경우 간접목적어가 뒤로 가면서 전치사(to,for,of)가 붙습니다.<br />
                      to를 취하는 동사 : give, send, teach, tell.. /for를 취하는 동사 : make, buy, get.. / of를 취하는 동사 : ask<br />
                    </li>
                    <li>
                      must : ~해야만 한다 (=have to) Ex): I must find him = I have to find him<br />
                              ~임에 틀림없다 Ex): He must be there = I'm sure/I'm certain he's there.<br />
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
          speech:'Excuse me. Do you have a book called Modern Banking?'
        },
        {
          name:'B:',
          speech:'I sold the last copy two months ago.'
        },
        {
          name:'A:',
          speech:'Did you order more copies of the book?'
        },
        {
          name:'B:',
          speech:'Yes, I did. Many people are asking for it.'
        },
        {
          name:'A:',
          speech:'How long ago did you order them?'
        },
        {
          name:'B:',
          speech:'About a week ago.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'Was Sam here today?'
        },
        {
          name:'D:',
          speech:'Yes, he was. He came for a haircut.'
        },
        {
          name:'C:',
          speech:'I must find him. Do you know where he went?'
        },
        {
          name:'D:',
          speech:'Yes. I think he went to the mall. It’s not far from here.'
        },
        {
          name:'C:',
          speech:'How long ago did he leave?'
        },
        {
          name:'D:',
          speech:'He left fifteen minutes ago. He must be there now.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'Excuse me. I left my glasses here this morning.'
        },
        {
          name:'F:',
          speech:'Where did you leave them?'
        },
        {
          name:'E:',
          speech:'Over there. I was at the table by the window.'
        },
        {
          name:'F:',
          speech:'Well, you’re lucky. The waiter found them about an hour ago.'
        },
        {
          name:'E:',
          speech:'Thank goodness! I was really worried.'
        },
        {
          name:'F:',
          speech:'There you go. He gave them to me a few minutes ago.'
        },
        {
          name:'E:',
          speech:'Yes. Those are mine. They’re new. I lost my last pair.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'실례합니다. Modern Banking이라는 책이 있나요?'
        },
        {
          name:'B:',
          speech:'두 달 전에 마지막 권을 팔았어요.'
        },
        {
          name:'A:',
          speech:'그 책을 더 주문했어요?'
        },
        {
          name:'B:',
          speech:'네, 그랬어요. 많은 사람들이 그것을 요구하고 있습니다.'
        },
        {
          name:'A:',
          speech:'주문한 지 얼마나 됐어요?'
        },
        {
          name:'B:',
          speech:'약 일주일 전에요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'C:',
          speech:'Sam 이 오늘 여기 있었나요?'
        },
        {
          name:'D:',
          speech:'네, 그랬어요. 그는 머리를 자르러 왔어요.'
        },
        {
          name:'C:',
          speech:'그를 찾아야 해요. 그가 어디로 갔는지 아세요?'
        },
        {
          name:'D:',
          speech:'네. 쇼핑몰에 간 것 같아요. 여기서 멀지 않아요.'
        },
        {
          name:'C:',
          speech:'얼마나 오래 전에 떠났나요?'
        },
        {
          name:'D:',
          speech:'그는 15분 전에 떠났습니다. 그는 지금 틀림없이 거기에 있을 거예요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'실례합니다. 오늘 아침에 안경을 두고 왔어요.'
        },
        {
          name:'F:',
          speech:'그것들을 어디에 두었습니까?'
        },
        {
          name:'E:',
          speech:'저기요. 창가 쪽 테이블에 있었어요.'
        },
        {
          name:'F:',
          speech:'운이 좋으시네요. 웨이터가 한 시간 전에 그들을 발견했어요.'
        },
        {
          name:'E:',
          speech:'다행이에요! 정말 걱정했어요.'
        },
        {
          name:'F:',
          speech:'여기 있습니다. 그는 몇 분 전 그것들을 나에게 줬어요.'
        },
        {
          name:'E:',
          speech:'네, 제 것입니다. 새것들이에요. 마지막 한 켤레를 잃어버렸어요.'
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
