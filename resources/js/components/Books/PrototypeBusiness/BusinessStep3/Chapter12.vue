<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/Lx6xU/MADySSLx6xU/1/s2/canva-man-and-woman-lying-on-mattress-MADySSLx6xU.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Talking about weekend 
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
          Tick the things that Dave did last weekend.
        </p>

        <ol style="margin: 12px;">
          <li>
            He sat in the garden. (&emsp;)
          </li>
          <li>
            He had some friends round. (&emsp;)
          </li>
          <li>
            He cooked a meal. (&emsp;)
          </li>
          <li>
            He did some gardening. (&emsp;)
          </li>
          <li>
            He worked on the house. (&emsp;)
          </li>
          <li>
            He had a lie in. (&emsp;)
          </li>
        </ol>

        <p>
           Free response:<br />
           Discuss with your teacher what you did last weekend, or what you normally do at the weekend.<br />
           Try to find five things that you did/normally do.
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
                  Useful language<br />
                  Did you have a good weekend? / What did you do at the weekend?<br />
                  I had a relaxing/busy weekend. / We had some friends round for dinner.<br />
                  I cooked a big meal on Saturday night. / I had a lie in on Sunday morning.<br />
                  I worked on the house all weekend.
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
          name:'Tessa:',
          speech:'So, did you have a good weekend, Dave?'
        },
        {
          name:'Dave:',
          speech:'Yeah, OK, thanks. It was nice to have some warm weather for a change. We ate outside yesterday, at lunchtime. We sat outside in the garden.'
        },
        {
          name:'Tessa:',
          speech:'Did you?'
        },
        {
          name:'Dave:',
          speech:'Yeah, We wanted to have a barbecue, actually, but I forgot to buy some charcoal, so…'
        },
        {
          name:'Tessa:',
          speech:'Oh, no. You didn’t have people coming round?'
        },
        {
          name:'Dave:',
          speech:'Oh, no. It was just me and my wife, so… it wasn’t too bad. In fact, I was quite pleased. Normally, when we have a barbecue, I do the cooking, you see. But otherwise my wife cooks, so…'
        },
        {
          name:'Tessa:',
          speech:'So you slept in the sun, and your wife did all the cooking!'
        },
        {
          name:'Dave:',
          speech:'Well… I wasn’t asleep – I had one eye open… so I could see when it was ready! No, actually, I had quite a busy weekend! I put a new front door on the house on Saturday. It was a bigger job than I thought, actually. I got up early on Saturday and worked all day. Then on Sunday, I got up early and painted it… What about you? What did you do?'
        },
        {
          name:'Tessa:',
          speech:'Not much really. We went to the cinema on Saturday night.'
        },
        {
          name:'Dave:',
          speech:'Oh yeah? What did you see?'
        },
        {
          name:'Tessa:',
          speech:'Oh, it wasn’t very good. It was that new film with…'
        },
        ],

        translations:[
        {
          name:'테사:',
          speech:'그래, 주말은 잘 보냈니, 데이브?'
        },
        {
          name:'데이브:',
          speech:'응, 고마워. 기분전환으로 따뜻한 날씨가 조금 있어서 좋았어. 우리는 어제 점심시간에 밖에서 밥을 먹었어. 우리는 정원에 밖에 앉아 있었어.'
        },
        {
          name:'테사:',
          speech:'그랬어?'
        },
        {
          name:'데이브:',
          speech:'응, 사실 우리는 바비큐 파티를 하고 싶었는데, 숯 사는 걸 까먹어서…'
        },
        {
          name:'테사:',
          speech:'아, 안돼. 사람들이 주위에 없었어?'
        },
        {
          name:'데이브:',
          speech:'오, 아니. 나와 내 아내뿐이었기 때문에 그리 나쁘지는 않았어. 사실, 나는 꽤 기뻤어. 보통은 바비큐를 할 때 내가 요리를 하지. 하지만 그렇지 않으면 아내가 요리를 해서…'
        },
        {
          name:'테사:',
          speech:'그러니까 햇빛 아래서 자고, 부인이 요리를 다 했구나!'
        },
        {
          name:'데이브:',
          speech:'글쎄, 난 잠을 못 잤어. 한 쪽 눈을 뜨고 있었어. 그래서 언제 그것이 준비되었는지 알 수 있었어! 아니, 사실, 나는 꽤 바쁜 주말을 보냈어! 토요일에 나는 집에 새 현관문을 놓았어. 생각했던 것보다 더 큰 일이었어. 토요일에는 일찍 일어나서 하루 종일 일했어. 그리고 일요일에는 일찍 일어나서 그림을 그렸어… 너는? 너는 뭐했어?'
        },
        {
          name:'테사:',
          speech:'별거 안했어. 우리는 토요일 밤에 영화관에 갔어.'
        },
        {
          name:'데이브:',
          speech:'오 그래? 뭘 봤니?'
        },
        {
          name:'테사:',
          speech:'아, 별로 좋지 않았어. 그 새로운 영화는....'
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
