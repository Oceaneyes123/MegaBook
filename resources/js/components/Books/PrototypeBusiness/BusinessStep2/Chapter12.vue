<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGv7jcIQA/6/screen_2x/canva-street-under-cloudy-sky-MADGv7jcIQA.jpg" class = "cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgba(254, 183, 43, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Making plans 1

      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border" >Today's topic</h3>
  <div style = "padding : 16px;">


        <table style = "border-collapse: collapse;">

          <tr v-for="dialog in dialogs" :key="dialog">
            <td class = "uppertable" >{{dialog.name}}</td>
            <td class = "lowertable" >{{dialog.speech}}</td>
          </tr>

        </table>


  <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Translation</h3>
      <div style="padding : 16px;">
    
          <table style = "border-collapse: collapse;">
    
            <tr v-for="translation in translations" :key="translation">
              <td class = "uppertable" >{{translation.name}}</td>
              <td class = "lowertable" >{{translation.speech}}</td>
            </tr>
    
          </table>
       </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Exercise</h3>
    <div style="padding : 16px;">

      <p>
        Put the words in order. Make sentences.
      </p>

      <ol style="margin: 12px;">
        <li>
          meeting/shall/where/have/we/the?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          go/by/to/train/the/let's/conference.<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          shall/when/visit/the/we/factory?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
      </ol>
      <p>
        Free response:<br />
        Work with a partner. Make suggestions about these things:
      </p>
      <p>
        - go for lunch.<br />
        - meet tomorrow<br />
        - talk next week<br />
        - discuss this now<br />
        - decide later<br />
        - put on the agenda
      </p>

    </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Self Study</h3>
    <div style="padding : 16px;">


      <p>
        Notes
      </p>

      <p>

        <v-container grid-list-md text-xs-left>
          <v-layout row wrap>


            <v-flex xs12>
              <v-card light color="#527318">
                <v-card-text class="px-10">
                  <p>
                    Making suggestions
                  </p>
                  <p>
                    <b>Shall+ I/we</b> + infinitive<br />
                    <b>Shall</b> we meet next month?<br />
                    <b>Shall</b> I call tomorrow?<br />
                    Where <b>shall</b> we meet?
                  </p>
                  <p>
                    Let's+ infinitive<br />
                    <b>Let's</b> go now.<br />
                    <b>Let's</b> meet next week.
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
          name:'Kristi:',
          speech:'So, where shall we meet?'
        },
        {
          name:'Akio:',
          speech:'Um...well, I can come to your office, or you can come here.'
        },
        {
          name:'Kristi:',
          speech:'Well, you came here last time, so shall I come to Tokyo?'
        },
        {
          name:'Akio:',
          speech:'Yes, OK. Yeah, then you can meet our new design manager.'
        },
        {
          name:'Kristi:',
          speech:'Oh, yes. Good idea. OK, so let’s meet in Tokyo.'
        },
        {
          name:'Akio:',
          speech:'OK. How many days do we need?'
        },
        {
          name:'Kristi:',
          speech:'Hmm...good question.'
        },
        {
          name:'Akio:',
          speech:'Shall we plan the meeting, first? Then we can decide when to meet, and how long we need...'
        },
        {
          name:'Kristi:',
          speech:'Yes, OK.'
        },
        {
          name:'Akio:',
          speech:'I wrote a list, this morning, of the things I’d like to look at with you.'
        },
        {
          name:'Kristi:',
          speech:'Right. Good.'
        },
        {
          name:'Akio:',
          speech:'So, um... well, Shall I email it to you? Then you can look at it, and we can talk later.'
        },
        {
          name:'Kristi:',
          speech:'Yes, OK, good idea. Let’s do that.'
        },
        {
          name:'Akio:',
          speech:'I’ll send it now. And I’ll call back, um... When shall I call you?'
        },
        {
          name:'Kristi:',
          speech:'Let’s talk again in an hour.'
        },
        {
          name:'Akio:',
          speech:'OK, fine. Bye.'
        },
        ],

        translations:[
        {
          name:'크리스티:',
          speech:'그럼, 어디서 만날까요?'
        },
        {
          name:'아키오:',
          speech:'음...요...음, 제가 당신 사무실로 갈 수도 있고, 아니면 당신이 여기로 올 수도 있어요.'
        },
        {
          name:'크리스티:',
          speech:'Well, you came here last time, so shall I come to Tokyo?'
        },
        {
          name:'아키오:',
          speech:'Yes, OK. Yeah, then you can meet our new design manager.'
        },
        {
          name:'크리스티:',
          speech:'Oh, yes. Good idea. OK, so let’s meet in Tokyo.'
        },
        {
          name:'아키오:',
          speech:'OK. How many days do we need?'
        },
        {
          name:'크리스티:',
          speech:'Hmm...good question.'
        },
        {
          name:'아키오:',
          speech:'Shall we plan the meeting, first? Then we can decide when to meet, and how long we need...'
        },
        {
          name:'크리스티:',
          speech:'Yes, OK.'
        },
        {
          name:'아키오:',
          speech:'I wrote a list, this morning, of the things I’d like to look at with you.'
        },
        {
          name:'크리스티:',
          speech:'Right. Good.'
        },
        {
          name:'아키오:',
          speech:'So, um... well, Shall I email it to you? Then you can look at it, and we can talk later.'
        },
        {
          name:'크리스티:',
          speech:'Yes, OK, good idea. Let’s do that.'
        },
        {
          name:'아키오:',
          speech:'I’ll send it now. And I’ll call back, um... When shall I call you?'
        },
        {
          name:'크리스티:',
          speech:'Let’s talk again in an hour.'
        },
        {
          name:'아키오:',
          speech:'OK, fine. Bye.'
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
  border-color: transparent #899857 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background: #899857;
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
