<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/people-working-call-center_23-2148094787.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 class="upper-header-BS3">Talking about your job 
      </h1>
    </v-layout>
  </v-img>

  <div class="top-line-BS3">
  </div>
  <h3  class = "lower-header-BS3 white--text" >Today's topic</h3>
  <div style = "padding : 16px;">

    <table style = "border-collapse: collapse;">

      <tr v-for="dialog in dialogs" :key="dialog">
        <td class = "uppertable" >{{dialog.name}}</td>
        <td class = "lowertable" >{{dialog.speech}}</td>
      </tr>

    </table>

    
    <div class = "line-BS3">
    </div>
    <h3 class = "border-BS3 white--text">Translation</h3>
    <div style="padding : 16px;">

      <table style = "border-collapse: collapse;">

        <tr v-for="translation in translations" :key="translation">
          <td class = "uppertable" >{{translation.name}}</td>
          <td class = "lowertable" >{{translation.speech}}</td>
        </tr>

      </table>
   </div>

      <div class = "line-BS3">
      </div>
      <h3 class = "border-BS3 white--text">Exercise</h3>
      <div style="padding : 16px;">

        <p>
          Fill in the gaps with these forms of the verb be.<br />
          <u>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;</u>
        </p>
        <p>
          are   is   I'm   he's   isn't   we're   they're   aren't   isn't<br />
          <u>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;</u>
        </p>


        <ol style="margin: 12px;">
          <li>
            A: My name’s Ella Grady. ( &emsp; &emsp; ) in customer service. It ( &emsp; &emsp; ) a very big department only six people.
          </li>
          <li>
            I’m not in charge of the department. David Kemp ( &emsp; &emsp; ) the manager. ( &emsp; &emsp; ) is my boss.
          </li>
          <li>
            I work with five colleagues. ( &emsp; &emsp; ) in the European section of the department.
          </li>
          <li>
            Sue Arpel ( &emsp; &emsp; ) on the course. There ( &emsp; &emsp; ) any directors on the course.
          </li>
        </ol>

        <p>
          Free response:<br />
          Talk about your company and your job.<br />
          What's your job title in English?<br />
          Is your job common or very specialised<br />
          Do you know anyone with a very unusual job?
        </p>

      </div>

      <div class = "line-BS3">
      </div>
      <h3 class = "border-BS3 white--text">Self Study</h3>
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
                      Present simple : be
                    </p>
                    <p>
                      I’<b>m</b> an expert manager.<br />
                      He’<b>s</b> in charge.<br />
                      We’<b>re</b> responsible for ten countries.<br />
                      I’<b>m not</b> in charge.<br />
                      She <b>isn’t</b> on the course.<br />
                      They <b>aren’t</b> all here.
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
          name:'Ella:',
          speech:'My name’s Ella Grady. I’m in the customer service department. I’m the European customer service manager. So, um… I look after customer service for Europe.'
        },
        {
          name:'Ivan:',
          speech:'So are you in charge of the department?'
        },
        {
          name:'Ella:',
          speech:'I’m not the department manager, no. I report to the customer service manager. He’s in charge of the department.'
        },
        {
          name:'David:',
          speech:'She reports to me!'
        },
        {
          name:'Ivan:',
          speech:'Ah! The boss is here!'
        },
        {
          name:'David:',
          speech:'I’m afraid so!'
        },
        {
          name:'Ivan:',
          speech:'And is your boss here?'
        },
        {
          name:'David:',
          speech:'No, she isn’t on the course. Fortunately!'
        },
        {
          name:'Ivan:',
          speech:'I see. So, Ella, you aren’t the department manager, but do you have a team… in the department?'
        },
        {
          name:'Ella:',
          speech:'Yeah, I manage a small team of assistants. Five people. They’re not all here – just two of them.'
        },
        {
          name:'Ivan:',
          speech:'Right. And how big is the region you look after?'
        },
        {
          name:'Ella:',
          speech:'We’re responsible for customers in Europe, um…eighteen countries, altogether.'
        },
        {
          name:'Ivan:',
          speech:'And do you have direct contact with customers? Do you speak to them?'
        },
        {
          name:'Ella:',
          speech:'oh yes. The difficult ones, usually! I deal with problems most of the time.'
        },
        {
          name:'Ivan:',
          speech:'So you deal with difficult customers?'
        },
        {
          name:'Ella:',
          speech:'Quite a lot, yes.'
        },
        {
          name:'David:',
          speech:'She has a difficult boss, as well!'
        },
        {
          name:'Ivan:',
          speech:'Oh, I see!'
        },
        ],

        translations:[
        {
          name:'엘라:',
          speech:'제 이름은 엘라 그래디입니다. 저는 고객 서비스 부서에 있습니다. 저는 유럽 고객 서비스 매니저입니다. 그래서, 음... 저는 유럽에 대한 고객 서비스를 관리합니다.'
        },
        {
          name:'이반:',
          speech:'그래서 당신이 그 부서를 책임지고 있는 건가요?'
        },
        {
          name:'엘라:',
          speech:'전 부장이 아닙니다. 저는 고객 서비스 매니저에게 보고합니다. 그는 그 부서를 책임지고 있습니다.'
        },
        {
          name:'데이비드:',
          speech:'그녀는 나에게 보고합니다!'
        },
        {
          name:'이반:',
          speech:'A아! 사장님이 오셨어요!'
        },
        {
          name:'데이비드:',
          speech:'유감스럽게도 그래!'
        },
        {
          name:'이반:',
          speech:'그리고 당신의 상사는 여기 있나요?'
        },
        {
          name:'데이비드:',
          speech:'아니요, 그녀는 그 과정에 있지 않아. 다행히도!'
        },
        {
          name:'이반:',
          speech:'그렇군요. 엘라, 당신은 부장이 아니시지만, 부서에 팀이 있으십니까?'
        },
        {
          name:'엘라:',
          speech:'네, 저는 작은 조수 팀을 운영하고 있어요. 다섯 명. 그들은 모두 여기에 있는 것이 아니에요. 단지 그들 중 두 명입니다.'
        },
        {
          name:'이반:',
          speech:'그렇군요. 그리고 당신이 돌보는 지역은 얼마나 큰가요?'
        },
        {
          name:'엘라:',
          speech:'우리는 유럽의 고객들을 책임지고 있어요. 음... 8개국의 국가들 모두요.'
        },
        {
          name:'이반:',
          speech:'그리고 손님들과 직접 접촉하는 건가요? 그들과 얘기하나요?'
        },
        {
          name:'엘라:',
          speech:'오 그래요. 보통 어려운 것들이죠. 저는 대부분의 문제를 다룹니다.'
        },
        {
          name:'이반:',
          speech:'오 그래요. 보통 어려운 것들이죠. 저는 대부분의 문제를 다룹니다.'
        },
        {
          name:'엘라:',
          speech:'네, 꽤 많이요.'
        },
        {
          name:'데이비드:',
          speech:'그녀에게도 어려운 상사가 있어요!'
        },
        {
          name:'이반:',
          speech:'아, 그렇구나!'
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
