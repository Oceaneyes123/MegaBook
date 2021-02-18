<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/price-tag-male-clothing-wooden-desk_23-2148189265.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Army recruiting office
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Army recruiting office</li><br />

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
          <u>Your friend is going to the army in Korea</u><br />
        </p>

        <ol style="margin: 12px;">
          <li>
            What will he have to do?
          </li>
          <li>
            What won’t he have to do?
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
                      get a hair : 머리를 깎다
                    </li>
                    <li>
                      wear a uniform : 유니폼을 입다                   
                    </li>
                    <li>
                      obey orders : 명령에 복종하다
                    </li>
                    <li>
                      there you go : 여기 있습니다
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
          name:'Corona:',
          speech:'Hi there. I want to join the army.'
        },
        {
          name:'Sergeant:',
          speech:'What! You! In the army?'
        },
        {
          name:'Corona:',
          speech:'Yeah. I want to be a soldier. This is the Army Recruiting Office, isn’t it?'
        },
        {
          name:'Sergeant:',
          speech:'Well, sit down, son. Now, why do you want to be a soldier?'
        },
        {
          name:'Corona:',
          speech:'Well, I saw the commercial on TV last night. It looked pretty good. Vacations, money, travel, education, a pension…'
        },
        {
          name:'Sergeant:',
          speech:'I see. Yes, it’s a good life in the army.'
        },
        {
          name:'Corona:',
          speech:'Terrific!'
        },
        {
          name:'Sergeant:',
          speech:'Now, do you have any questions?'
        },
        {
          name:'Corona:',
          speech:'Let’s see. Yes. Will I have to get a haircut?'
        },
        {
          name:'Sergeant:',
          speech:'Oh yes, you’ll have to get a haircut — and wear a uniform.'
        },
        {
          name:'Corona:',
          speech:'A uniform? I’ve never had to wear a uniform before.'
        },
        {
          name:'Sergeant:',
          speech:'Oh yes, and you’ll have to obey orders. But you won’t have to clean toilets, ha-ha.'
        },
        {
          name:'Corona:',
          speech:'Hmm. And what about education?'
        },
        {
          name:'Sergeant:',
          speech:'Oh, yes. There are a lot of opportunities. Maybe you’ll be a computer programmer or a communications expert one day.'
        },
        {
          name:'Corona:',
          speech:'OK. I’d like to join.'
        },
        {
          name:'Sergeant:',
          speech:'All right. Just sign here.'
        },
        {
          name:'Corona:',
          speech:'There you go, man — Danny Corona.'
        },
        {
          name:'Sergeant:',
          speech:'CORONA!!!'
        },
        {
          name:'Corona:',
          speech:'Huh?'
        },
        {
          name:'Sergeant:',
          speech:'Stand up! Stand up straight, Corona. Now, march! Left, right, left, right. You’re in the army now!'
        },
        ],

        translations:[
        {
          name:'Corona:',
          speech:'안녕하세요. 군대에 가고 싶어요.'
        },
        {
          name:'병장:',
          speech:'뭐라고요! 당신! 군대에?'
        },
        {
          name:'Corona:',
          speech:'네. 저는 군인이 되고 싶습니다. 여기가 육군 모병소죠?'
        },
        {
          name:'병장:',
          speech:'앉아요, 청년. 자, 왜 군인이 되고 싶습니까?'
        },
        {
          name:'Corona:',
          speech:'음, 어젯밤에 TV에서 광고를 봤어요. 꽤 좋아 보였어요. 휴가, 돈, 여행, 교육, 연금 같은 거요.'
        },
        {
          name:'병장:',
          speech:'그렇군요. 네, 군생활이 좋네요.'
        },
        {
          name:'Corona:',
          speech:'멋져요!'
        },
        {
          name:'병장:',
          speech:'자, 질문 있으신가요?'
        },
        {
          name:'Corona:',
          speech:'어디 봐요. 네. 머리를 잘라야 하나요?'
        },
        {
          name:'병장:',
          speech:'네, 머리를 자르고 군복을 입어야 합니다.'
        },
        {
          name:'Corona:',
          speech:'군복이요? 저는 한 번도 군복을 입어야 했던 적이 없어요.'
        },
        {
          name:'병장:',
          speech:'네, 그리고 명령에 복종해야 할 거예요. 하지만 화장실 청소는 안 해도 돼요, 하하'
        },
        {
          name:'Corona:',
          speech:'음.요. 그렇다면 교육은 어떨까요?'
        },
        {
          name:'병장:',
          speech:'아 기회는 많습니다. 언젠가는 컴퓨터 프로그래머나 통신 전문가가 될 수도 있겠죠.'
        },
        {
          name:'Corona:',
          speech:'알겠습니다. 저도 입대하고 싶어요.'
        },
        {
          name:'병장:',
          speech:'좋아요. 여기에 서명만 하시면 됩니다.'
        },
        {
          name:'Corona:',
          speech:'여기 있습니다. Danny Corona.'
        },
        {
          name:'병장:',
          speech:'Corona!!!!!'
        },
        {
          name:'Corona:',
          speech:'네?'
        },
        {
          name:'병장:',
          speech:'일어서요! 똑바로 서요, Corona. 자, 행진하세요! 왼쪽, 오른쪽, 왼쪽, 오른쪽. 당신은 지금 군대에 있어요!'
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
