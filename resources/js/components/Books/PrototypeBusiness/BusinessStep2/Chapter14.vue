<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGv1kRgZ4/7/screen_2x/canva-woman-standing-near-whiteboard-MADGv1kRgZ4.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Describing plans 1
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border" >Today's topic</h3>
  <div style = "padding : 16px;">

    <p>
      Extract 1<br />
      </p>
      <br />
    <table style = "border-collapse: collapse;">

      <tr v-for="firstextractdialog in firstextractdialogs" :key="firstextractdialog">
        <td class = "uppertable" >{{firstextractdialog.name}}</td>
        <td class = "lowertable" >{{firstextractdialog.speech}}</td>
      </tr>

    </table>

        <br />
        <p>
        Extract 2<br />
        </p>
        <br />

          
        <table style = "border-collapse: collapse;">

          <tr v-for="secondextractdialog in secondextractdialogs" :key="secondextractdialog">
            <td class = "uppertable" >{{secondextractdialog.name}}</td>
            <td class = "lowertable" >{{secondextractdialog.speech}}</td>
          </tr>
    
        </table>


<div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Translation</h3>
    <div style="padding : 16px;">

      <p>
        Extract 1<br />
        </p>
        <br />

      <table style = "border-collapse: collapse;">


        <tr v-for="firstextracttranslation in firstextracttranslations" :key="firstextracttranslation">
          <td class = "uppertable" >{{firstextracttranslation.name}}</td>
          <td class = "lowertable" >{{firstextracttranslation.speech}}</td>
        </tr>

      </table>

      <br />
      <p>
      Extract 2<br />
      </p>
      <br />


      <table style = "border-collapse: collapse;">


        <tr v-for="secondextracttranslation in secondextracttranslations" :key="secondextracttranslation">
          <td class = "uppertable" >{{secondextracttranslation.name}}</td>
          <td class = "lowertable" >{{secondextracttranslation.speech}}</td>
        </tr>

      </table>


   </div>

  
    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Exercise</h3>
    <div style="padding : 16px;">

      <p>
        Make sentences with going to.
      </p>

      <ol style="margin: 12px;">
        <li>
          where/ they/ meet?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          what/ she/ present/ at the conference?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
        <li>
          you/ work/ late/ tonight?<br />
          ( &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; )
        </li>
      </ol>
      <p>
        Free response:<br />
        What are you going to do next week?<br />
        On... I'm going to ... .
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
                    Future with going to<br />
                    긍정문<br />
                    I'<b>m going</b> to discuss the plan.
                  </p>
                  <p>
                    의문형<br />
                    <b>Are</b> you <b>going to</b> discuss the website?
                  </p>
                  <p>
                    부정문<br />
                    We'<b>re not going</b> to talk about the website.
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
        firstextractdialogs:[
        {
          name:'Kristi:',
          speech:'Er... we’re going to look at the website, as well.'
        },
        {
          name:'Simon:',
          speech:'Right. I wanted to ask you about that. What’s the plan for the website, exactly?'
        },
        {
          name:'Kristi',
          speech:'Well, I want to change the design. Um...'
        },
        {
          name:'Simon:',
          speech:'Completely?'
        },
        {
          name:'Kristi:',
          speech:'I think we need to make some big changes, yes.'
        },
        {
          name:'Simon:',
          speech:'Why? What’s the... what’s the aim?'
        },
        {
          name:'Kristi:',
          speech:'Well, we need to make it easier to use. Um... that’s the main objective.'
        },
        {
          name:'Simon:',
          speech:'Right.'
        },
        ],

        secondextractdialogs:[
        {
          name:'Simon:',
          speech:'OK, good. When are you going to have it ready? What’s your target date?'
        },
        {
          name:'Kristi:',
          speech:'Well. our aim is to have the new site online this year... before the end of the year. ... That’s our goal.'
        },
        ],

        firstextracttranslations:[
        {
          name:'크리스티:',
          speech:'음... . 어, 그래요. 우리도 웹사이트를 살펴볼 것입니다.'
        },
        {
          name:'사이먼:',
          speech:'맞아요. 그것에 대해 물어보고 싶었어요. 웹사이트 계획은 정확히 어떻게 되나요?'
        },
        {
          name:'크리스티:',
          speech:'음, 저는 디자인을 바꾸고 싶어요. 음.. 제가..'
        },
        {
          name:'사이먼:',
          speech:'완전히요?'
        },
        {
          name:'크리스티:',
          speech:'저는 우리가 큰 변화를 만들어야 한다고 생각해요, 그렇죠.'
        },
        {
          name:'사이먼:',
          speech:'왜요? 그게 뭐에요? 목적이 뭐죠?'
        },
        {
          name:'크리스티:',
          speech:'음, 우리는 그것을 사용하기 쉽게 만들어야 합니다. 음... 그게 주된 목표입니다.'
        },
        {
          name:'사이먼',
          speech:'그렇군요.'
        },
        ],

        secondextracttranslations:[
        {
          name:'사이먼:',
          speech:'좋아요. 언제 그것을 준비하실 건가요? 목표 날짜가 언제입니까?'
        },
        {
          name:'크리스티:',
          speech:'음. 저희의 목표는 올해 새로운  온라인사이트를 가지는 것입니다. 올해가 끝나기 전에 말이죠... 그게 우리의 목표입니다.'
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
