<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/woman-washing-head-hairsalon_1157-27179.jpg" class="cover-photo">

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
        padding-bottom: 10px;">I had to wash my hair…
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">I had to wash my hair…</li><br />

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
            Why’s Randy calling Vicky?<br />
          </li>
          <li>
            Why couldn’t Vicky come?<br />
          </li>
          <li>
            Why did she have to wash her hair?<br />
          </li>
          <li>
            Is she going to the theater with Randy?<br />
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
                      조동사 : have to - ~해야만 한다 (과거: had to - ~해야만 했다)<br />
                              can - ~할 수 있다 (과거: could : ~할 수 있었다)<br />
                              <br />
                              Ex) I couldn't remember your phone number : 나는 너의 전화번호를 기억할 수 없었다./<br />
                              Why did you have to wash your hair last night? : 너는 왜 어젯밤에 머리를 감아야 했니?<br />
                              I had to do it last night because I'm going to see a play tonight : 나는 오늘밤에 연극을 보러 가기 때문에 어젯밤에 그것을 해야만 했어<br />
                              I couldn't say no : 안 된다고 말할 수 없었어<br />
                    </li>
                    <li>
                      to부정사 : 문장에서 주어나 목적어, 보어 역할을 합니다<br />
                              I wanted to call you : 나는 너에게 전화 하기를 원했어.<br />
                    </li>
                    <li>
                      What do you mean? : 무슨 말씀이세요?<br />
                    </li>
                    <li>
                      to wait for ~ : 기다리다<br />
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
          name:'Vicky:',
          speech:'Hello?'
        },
        {
          name:'Randy:',
          speech:'Vicky? Is that you?'
        },
        {
          name:'Vicky:',
          speech:'Uh-huh. Who’s this?'
        },
        {
          name:'Randy:',
          speech:'It’s Randy.'
        },
        {
          name:'Vicky:',
          speech:'Randy? Randy who?'
        },
        {
          name:'Randy:',
          speech:'What do you mean, "Randy who?" Randy Dixon, of course.'
        },
        {
          name:'Vicky:',
          speech:'Oh, Randy, I’m sorry.'
        },
        {
          name:'Randy:',
          speech:'Yes. We had a date last night. Where were you? I waited for two hours.'
        },
        {
          name:'Vicky:',
          speech:'Oh, I’m sorry, Randy. I couldn’t come.'
        },
        {
          name:'Randy:',
          speech:'Couldn’t come! Why not?'
        },
        {
          name:'Vicky:',
          speech:'Well, I had to wash my hair.'
        },
        {
          name:'Randy:',
          speech:'Wash your hair! Why didn’t you call me?'
        },
        {
          name:'Vicky:',
          speech:'I wanted to call you, but—uh—I couldn’t remember your phone number.'
        },
        {
          name:'Randy:',
          speech:'It’s in the phone book.'
        },
        {
          name:'Vicky:',
          speech:'Yes, of course, but—uh— I couldn’t remember your last name.'
        },
        {
          name:'Randy:',
          speech:'Oh… But why did you have to wash your hair last night?'
        },
        {
          name:'Vicky:',
          speech:'Well, I had to do it last night because I’m going to see a play tonight.'
        },
        {
          name:'Randy:',
          speech:'To see a play? With who?'
        },
        {
          name:'Vicky:',
          speech:'George. George McQueen, my boss’s son.'
        },
        {
          name:'Randy:',
          speech:'I see.'
        },
        {
          name:'Vicky:',
          speech:'He asked me yesterday, and I couldn’t say no.'
        },
        ],

        translations:[
        {
          name:'Vicky:',
          speech:'여보세요?'
        },
        {
          name:'Randy:',
          speech:'Vicky요? 당신인가요?'
        },
        {
          name:'Vicky:',
          speech:'어, 그래요. 누구죠?'
        },
        {
          name:'Randy:',
          speech:'Randy예요.'
        },
        {
          name:'Vicky:',
          speech:'Randy요? Randy 누구요?'
        },
        {
          name:'Randy:',
          speech:'"Randy who"라니요? Randy Dixon, 물론이죠.'
        },
        {
          name:'Vicky:',
          speech:'아, Randy, 미안해요.'
        },
        {
          name:'Randy:',
          speech:'그래요. 우리는 어젯밤에 데이트를 했어요. 어디 있었어요? 두 시간이나 기다렸어요.'
        },
        {
          name:'Vicky:',
          speech:'오, 미안해요, Randy. 올 수 없었어요.'
        },
        {
          name:'Randy:',
          speech:'올 수 없었어요! 왜 안되죠?'
        },
        {
          name:'Vicky:',
          speech:'음, 머리를 감아야 했어요.'
        },
        {
          name:'Randy:',
          speech:'머리를 감으세요! 왜 전화 안 했어요?'
        },
        {
          name:'Vicky:',
          speech:'전화하고 싶었는데, 음, 전화번호를 기억할 수가 없었어요..'
        },
        {
          name:'Randy:',
          speech:'전화번호부에 있어요.'
        },
        {
          name:'Vicky:',
          speech:'네, 물론이죠, 하지만, 음. 저는 당신의 성을 기억할 수 없었어요'
        },
        {
          name:'Randy:',
          speech:'아…그런데 왜 어젯밤에 머리를 감아야 했나요?'
        },
        {
          name:'Vicky:',
          speech:'음, 어젯밤에 해야 했어요. 오늘 밤에 연극을 보러 갈 예정이라서요.'
        },
        {
          name:'Randy:',
          speech:'연극 보러요? 누가요?으로'
        },
        {
          name:'Vicky:',
          speech:'George요. George McQueen, 제 상사의 아들이죠'
        },
        {
          name:'Randy:',
          speech:'알겠습니다.'
        },
        {
          name:'Vicky:',
          speech:'그가 어제 나에게 물었고, 나는 거절할 수 없었어요.'
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
