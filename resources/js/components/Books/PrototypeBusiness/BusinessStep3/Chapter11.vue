<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/hx8Fw/MADyQ7hx8Fw/1/s2/canva-photo-of-man-holding-camera-MADyQ7hx8Fw.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgba(140, 103, 90, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Discussing past projects
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color:#402B24; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border white--text" >Today's topic</h3>
  <div style = "padding : 16px;">

    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table> 

    
    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #402B24; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #402B24;">Translation</h3>
    <div style="padding : 16px;">

      <table style = "border-collapse: collapse;">

        <tr v-for="translation in translations" :key="translation">
          <td class = "uppertable" >{{translation.name}}</td>
          <td class = "lowertable" >{{translation.speech}}</td>
        </tr>

      </table>
   </div>


      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Exercise</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>
            What was the first problem Jake had?
          </li>
          <li>
            What was the solution?
          </li>
          <li>
            What was the second problem?
          </li>
          <li>
            Was it possible to solve the problem?
          </li>
        </ol>

        <p>
           Free response:<br />
           Talk about a project you worked on.<br />
           What problem did you have?<br />
           How did you solve them?
        </p>

      </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Self Study</h3>
      <div style="padding : 16px;">


          <p>
            Notes
          </p>

        <p>

          <v-container grid-list-md text-xs-left>
            <v-layout row wrap>


              <v-flex xs12>
                <v-card light color="#F2CBBD">
                  <v-card-text class="px-10">
                <p>
                  <b>Be:</b> past simple<br />
                  <b>Was</b> the product successful?<br />
                  No, it <b>wasn’t.</b> It <b>was</b> a flop.<br />
                  <b>Were</b> the products successful?<br />
                  No, they <b>weren’t</b> Sales <b>were</b> very low.
                </p>
                <p>
                  - Positive: We start<b>ed</b> the project in February. (regular)<br />
                  &emsp; &emsp; &emsp;&emsp; It <b>took</b> eleven months. (irregular)<br />
                  - Negative: The work <b>didn’t take</b> long. We <b>didn’t finish</b> on time.<br />
                  - Questions: When <b>did</b> you <b>start</b> the project?<br />
                  &emsp; &emsp;&emsp;&emsp;&emsp; <b>Did</b> it <b>take</b> long?
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
          name:'Jake:',
          speech:'So this is quite an easy project… certainly compared with the one we did last month, at a chemicals factory. It was, um… quite a challenge!'
        },
        {
          name:'Client:',
          speech:'At a chemicals factory?'
        },
        {
          name:'Jake:',
          speech:'Yeah. It was a marketing video, for a chemicals company. They wanted to film different…parts of the factory. The first problem was the heat. It was… I don’t know what the temperature was, exactly, but it was extremely hot.'
        },
        {
          name:'Client:',
          speech:'So it was difficult to work?'
        },
        {
          name:'Jake:',
          speech:'Well, the trouble was, it was too hot for the camera.'
        },
        {
          name:'Client:',
          speech:'Oh, right. So what did you do?'
        },
        {
          name:'Jake:',
          speech:'We put the camera in a box, to protect it. We made a box, with a small hole in the front..'
        },
        {
          name:'Client:',
          speech:'Yeah.'
        },
        {
          name:'Jake:',
          speech:'And we filmed with the camera in the box.'
        },
        {
          name:'Client:',
          speech:'And did it work?'
        },
        {
          name:'Jake:',
          speech:'Yeah, it worked OK.'
        },
        {
          name:'Client:',
          speech:'So how did you make the box? What did you use?'
        },
        {
          name:'Jake:',
          speech:'Just wood. Nothing complicated. So, anyway, we finished filming in this hot area… and then they wanted us to film with no light. They had another production process where, um… they couldn’t have any light at all. It was completely black.'
        },
        {
          name:'Client:',
          speech:'And they wanted you to film it?'
        },
        {
          name:'Jake:',
          speech:'Yeah.'
        },
        {
          name:'Client:',
          speech:'So what did you say?'
        },
        {
          name:'Jake:',
          speech:'I said, no, it’s impossible. They thought maybe we could use a special camera or something, but, um… it wasn’t possible. So, filming in your offices isn’t a big problem!'
        },
        {
          name:'Client:',
          speech:'Well after that, no! So, when can you start setting up…'
        },
        ],

        translations:[
        {
          name:'제이크:',
          speech:'이건 꽤 쉬운 프로젝트입니다. 확실히 지난 달에 화학 공장에서 했던 것과 비교하면. 그건, 음... 꽤 어려운 일이었어요!'
        },
        {
          name:'고객:',
          speech:'화학 공장에서요?'
        },
        {
          name:'제이크:',
          speech:'네. 그것은 한 화학 회사를 위한 마케팅 비디오였어요. 그들은 공장의 다른 부분들을 촬영하고 싶어했어요. 첫 번째 문제는 더위였어요. 정확히는 기온이 몇 도인지 모르겠지만, 엄청나게 더웠어요.'
        },
        {
          name:'고객:',
          speech:'그럼 일하는 게 어려웠다는 건가요?'
        },
        {
          name:'제이크:',
          speech:'글쎄, 문제는, 카메라한테 너무 뜨거워서 그랬어요.'
        },
        {
          name:'고객:',
          speech:'아, 맞다. 그래서 어떻게 하셨어요?'
        },
        {
          name:'제이크:',
          speech:'우리는 카메라를 상자에 넣었어요, 그것을 보호하기 위해서. 우리는 상자를 만들었고, 앞쪽에 작은 구멍이 있었어요.'
        },
        {
          name:'고객:',
          speech:'네.'
        },
        {
          name:'제이크:',
          speech:'그리고 우리는 상자에 있는 카메라로 촬영했어요.'
        },
        {
          name:'고객:',
          speech:'그리고 효과가 있었나요?'
        },
        {
          name:'제이크:',
          speech:'그래요, 잘 됐어요.'
        },
        {
          name:'고객:',
          speech:'그래서 어떻게 상자를 만들었나요? 무엇을 사용하셨습니까?'
        },
        {
          name:'제이크:',
          speech:'그냥 나무예요. 복잡한 건 없어요. 그래서 어쨌든, 우리는 이 더운 곳에서 촬영을 끝냈어요. 그들은 빛도 없이 찍기를 원했어요. 그들은 전혀 빛을 낼 수 없는 또 다른 생산 공정을 가졌어요. 완전히 검은 색이었어요.'
        },
        {
          name:'고객:',
          speech:'그리고 그들은 당신이 찍어주길 원했나요?'
        },
        {
          name:'제이크:',
          speech:'네.'
        },
        {
          name:'고객:',
          speech:'그래서 뭐라고 하셨어요?'
        },
        {
          name:'제이크:',
          speech:'불가능하다고 말했어요. 그들은 우리가 특별한 카메라 같은 것을 사용할 수 있다고 생각했지만, 음… 그건 불가능했어요. 그래서, 사무실에서 촬영하는 것은 큰 문제가 되지 않아요!'
        },
        {
          name:'고객:',
          speech:'음, 그 후로는 안돼요! 그럼 언제부터 설치하시겠습니까?'
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
  border-color: transparent#402B24 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background:#402B24;
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
