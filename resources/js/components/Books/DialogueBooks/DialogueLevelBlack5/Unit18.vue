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
        padding-bottom: 10px;">UFO - part 2
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">UFO - part 2</li><br />

      <br />
      <p>
        Dick and Jane were sitting in their car. Suddenly there was a loud noise, and a big, bright silver object flew low over them. It stopped in midair, turned around, and flew back over their car. Then it went straight up into the sky and disappeared.<br />
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
          Ex) Was it a UFO? (He has no idea)   >   He has no idea if it was a UFO.
        </p>

        <ol style="margin: 12px;">
          <li>
            Was it a dream? (We don’t know.)  >
          </li>
          <li>
            Where did the object go? (She doesn’t know.)  >
          </li>
          <li>
            Did it come from another planet? (She wonders) >
          </li>
          <li>
            Will the police believe them? (She has no idea.)  >
          </li>
          <li>
            What will the police say? (They wonder.)  >
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

        <p>
          Dick 과 Janet은 그들의 차에 앉아 있었습니다. 갑자기 큰 소리가 났고, 크고 밝은 은색 물체가 그들 위로 낮게 날아갔습니다. 그것은 공중에서 멈추고 돌아서서 그들의 차 위로 다시 날아갔습니다. 그리고는 곧장 하늘로 올라가 사라졌습니다.
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
                      I wonder why it wasn't working (그것이 왜 작동하지 않는지 궁금하다) : I wonder. + Why wasn't it working?<br />                 
                    </li>
                    <li>
                      Do you think it was a UFO? (그것이 UFO라고 생각하니?) : Do you think? + Was it a UFO?
                    </li>
                    <li>
                      Do you think they'll believe us? (너는 그들이 우리를 믿을 거라 생각하니?) : Do you think? Will they believe us?
                    </li>
                    <li>
                      It stopped in mid air : 그것이 상공에 멈췄다
                    </li>
                    <li>
                      turn around : 반대쪽으로 방향을 바꾸다
                    </li>
                    <li>
                      It went straight up into the sky : 하늘로 바로 올라갔다
                    </li>
                    <li>
                      I have no idea what it was - 그것이 무엇이었는지 모르겠어
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
          name:'Janet:',
          speech:'Wow! What was that?'
        },
        {
          name:'Dick:',
          speech:'Huh? Don’t ask me. I have no idea what it was.'
        },
        {
          name:'Janet:',
          speech:'Whew! Let’s go.'
        },
        {
          name:'Dick:',
          speech:'We can’t. The car won’t start.'
        },
        {
          name:'Janet:',
          speech:'Try it again.'
        },
        {
          name:'Dick:',
          speech:'That’s strange. It’s OK now. I wonder why it wasn’t working.'
        },
        {
          name:'Janet:',
          speech:'Do you think it was a UFO?'
        },
        {
          name:'Dick:',
          speech:'I have no idea if it was a UFO or something else. We should call the police.'
        },
        {
          name:'Janet:',
          speech:'Do you think they’ll believe us?'
        },
        ],

        translations:[
        {
          name:'Janet:',
          speech:'와우! 그게 뭐였어요?'
        },
        {
          name:'Dick:',
          speech:'네? 저한테 묻지 마세요. 저는 그게 무엇이었는지 전혀 모르겠어요.'
        },
        {
          name:'Janet:',
          speech:'휴! 가죠.'
        },
        {
          name:'Dick:',
          speech:'우리는 갈 수 없어요. 차가 시동이 안 걸려요.'
        },
        {
          name:'Janet:',
          speech:'다시 해 보세요.'
        },
        {
          name:'Dick:',
          speech:'이상하군요. 이제 괜찮아요. 왜 안 됐는지 궁금하네요.'
        },
        {
          name:'Janet:',
          speech:'UFO였다고 생각하세요?'
        },
        {
          name:'Dick:',
          speech:'저는 그것이 UFO인지 아니면 다른 것인지 전혀 모릅니다. 경찰을 불러야겠어요.'
        },
        {
          name:'Janet:',
          speech:'그들이 우리를 믿을까요?'
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
