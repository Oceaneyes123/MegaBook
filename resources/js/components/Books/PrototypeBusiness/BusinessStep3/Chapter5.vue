<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/iZlaI/MADyQ2iZlaI/1/s2/canva-man-and-woman-having-a-meeting-in-the-office-MADyQ2iZlaI.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Discussing strengths and weaknesses
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

        <p>
          Answer the questions.
        </p>

        <ol style="margin: 12px;">
          <li>
            Where does Marco work?
          </li>
          <li>
            What are his main strengths?
          </li>
          <li>
            What’s the problem with making him the manager?
          </li>
          <li>
            Do you think Judith and Rowan agree about Marco?
          </li>
        </ol>

        <p>
           Free response:<br />
           - Talk about the skills and characteristics you need in your job or a job you would like to have.<br />
           - What skills and characteristics do people need for these jobs? Give your opinion.<br />
           They need to be/be good at...<br />
           They need to like/enjoy...<br />
           (engineers, salespeople, fashion designers, politicians, chief executives)
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
                  Gerund
                </p>
                <p>
                  He’s <b>good at</b> solv<b>ing</b> problems.<br />
                  I’m <b>not very good at</b> mak<b>ing</b> presentations.<br />
                  They <b>like/enjoy</b> work<b>ing</b> here<br />
                  (gerund after verbs of like/dislike)<br />
                  Manag<b>ing</b> a big department isn’t easy.
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
          name:'Judith:',
          speech:'Marco works for PAF, he’s in the creative department, we know him, he knows us… But is that an advantage?'
        },
        {
          name:'Rowan:',
          speech:'Well, we want someone to manage the department. We need a manager to make the new strategy work. We don’t really need new ideas. Marco’s experienced, he knows the company well, and he knows what we want. I think his experience with PAF is a big advantage. Hiring someone new is… it’s obviously a risk.'
        },
        {
          name:'Judith:',
          speech:'Yeah. But making Marco the department manager’s also a risk. OK, he enjoys working for the company, he’s popular in the department, but… that doesn’t mean he’s good at managing a team.'
        },
        {
          name:'Rowan:',
          speech:'But the number one priority is the new strategy. The manager has to sell the new strategy to the team. We know Marco’s a good salesman. He likes selling ideas.'
        },
        {
          name:'Judith:',
          speech:'Yeah… But, what about the other people in the department? They work with him at the moment. What happens if they have to work for him?'
        },
        {
          name:'Rowan:',
          speech:'Oh, I think he can cope with all that…'
        },
        ],

        translations:[
        {
          name:'주디스:',
          speech:'마르코는 PAF에서 일합니다. 그는 창의적인 부서에서 일합니다. 우리는 그를 알고 있고, 그는 우리를 알고 있습니다. 하지만 그게 장점일까요?'
        },
        {
          name:'로완:',
          speech:'음, 우리는 누군가가 그 부서를 관리해주길 원해요. 우리는 새로운 전략을 실행하기 위해 매니저가 필요합니다. 우리는 새로운 아이디어가 별로 필요하지 않습니다. 마르코는 경험이 있고 회사를 잘 알아요. 우리가 뭘 원하는지 알고 있어요. 저는 그의 PAF 경험이 큰 장점이라고 생각합니다. 새로운 사람을 고용하는 것은 분명히 위험합니다.'
        },
        {
          name:'주디스:',
          speech:'그래요. 하지만 마르코를 부서장으로 만드는 것도 위험해요. 좋아요, 그는 회사에서 일하는 것을 즐기고, 부서에서 인기가 많아요. 그렇다고 해서 팀을 잘 운영한다는 뜻은 아닙니다.'
        },
        {
          name:'로완:',
          speech:'하지만 최우선 과제는 새로운 전략입니다. 매니저는 새로운 전략을 팀에 팔아야 합니다. 우리는 마르코가 훌륭한 세일즈맨이라는 것을 알고 있습니다. 그는 아이디어 파는 것을 좋아합니다.'
        },
        {
          name:'주디스:',
          speech:'네, 하지만, 부서의 다른 사람들은 어떤가요? 그들은 지금 그와 함께 일합니다. 만약 그들이 그를 위해 일해야 한다면 어떻게 될까요?'
        },
        {
          name:'로완:',
          speech:'아, 제 생각에 그는 그 모든 것에 대처할 수 있을 것 같아요...'
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
