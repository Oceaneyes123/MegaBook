<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/A8cak/MADzhTA8cak/1/s2/canva-people-walking-on-park-MADzhTA8cak.jpg" class = "cover-photo"> 

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
        padding-bottom: 10px;">Discussing how business is going

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
        Works in pairs. Discuss these sentences. Are they true for you?
      </p>

    <p>
      I work hard every day.<br />
      I prefer to work slowly and quickly.<br />
      I work well in a team.<br />
      I solve problems quickly.<br />
      Free response:<br />
      How's business at your company, or another company you know?
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
                    Adverbs of manner
                  </p>
                  <p>
                    Most adverbs of manner end in -ly:<br />
                    slow>slowly<br />
                    quick>quickly
                  </p>
                  <p>
                    These adverbs of manner are irregular:<br />
                    good>well<br />
                    hard>hard (no change)<br />
                    fast>fast (no change)
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
          name:'A:',
          speech:' So, how’s business in Vienna?'
        },
        {
          name:'B:',
          speech:' Um... improving.'
        },
        {
          name:'A:',
          speech:'Yeah?'
        },
        {
          name:'B:',
          speech:'Yeah, slowly. It’s um... It’s easier than last year.'
        },
        {
          name:'A:',
          speech:'Yeah.'
        },
        {
          name:'B:',
          speech:'We had a hard year, last year.'
        },
        {
          name:'A:',
          speech:'Low sales?'
        },
        {
          name:'B:',
          speech:'Well, we sold a lot of products. But, um... nearly all low-margin goods.'
        },
        {
          name:'A:',
          speech:'We had exactly the same situation in Dublin.'
        },
        {
          name:'B:',
          speech:'Last year?'
        },
        {
          name:'A:',
          speech:'Yeah. We made a profit-just.'
        },
        {
          name:'B:',
          speech:'We lost money.'
        },
        {
          name:'A:',
          speech:'Did you?'
        },
        {
          name:'B:',
          speech:'Yeah. Not too much, but, um...'
        },
        {
          name:'A:',
          speech:'But this year, you’re doing OK?'
        },
        {
          name:'B:',
          speech:'Yeah, we’re making money.'
        },
        {
          name:'A:',
          speech:'That’s good. We are. The good thing is, costs are lower this year, with the stronger euro.'
        },
        {
          name:'B:',
          speech:'That’s true, yeah. And they’re getting lower. Of course, you’re in the euro zone, in Ireland.'
        },
        {
          name:'A:',
          speech:'That’s right.'
        },
        {
          name:'B:',
          speech:'So, do you just manage one store?'
        },
        {
          name:'A:',
          speech:'Yeah, the Dublin branch. There is another one, in...'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'비엔나에서의 사업은 어때요?'
        },
        {
          name:'B:',
          speech:'음...요. 개선되는'
        },
        {
          name:'A:',
          speech:'그래요?'
        },
        {
          name:'B:',
          speech:'네, 천천히요. 그건 음... 그래요. 작년보다 쉬워요.'
        },
        {
          name:'A:',
          speech:'그래요.'
        },
        {
          name:'B:',
          speech:'작년에는 힘든 한 해를 보냈어요.'
        },
        {
          name:'A:',
          speech:'매출이 적어요?'
        },
        {
          name:'B:',
          speech:'음, 우리는 많은 제품을 팔았어요. 하지만, 음, 음... 거의 값싼 상품입니다.'
        },
        {
          name:'A:',
          speech:'더블린에서도 똑같은 상황이 있었어요.'
        },
        {
          name:'B:',
          speech:'작년에요?'
        },
        {
          name:'A:',
          speech:'그래요. 우리는 이윤을 추구했어요.'
        },
        {
          name:'B:',
          speech:'우리는 돈을 잃었어요.'
        },
        {
          name:'A:',
          speech:'그랬어요?'
        },
        {
          name:'B:',
          speech:'그래요. 너무 많지는 않지만, 음, 음... 괜찮아요.'
        },
        {
          name:'A:',
          speech:'하지만 올해는 잘 지내고 있어요?'
        },
        {
          name:'B:',
          speech:'네, 우리는 돈을 벌고 있어요.'
        },
        {
          name:'A:',
          speech:'잘됐네요. 우리는 그래요. 좋은 점은 유로가 강세를 보이면서 올해는 비용이 더 낮아졌다는 점입니다.'
        },
        {
          name:'B:',
          speech:'맞아요. 점점 낮아지고 있습니다. 물론, 당신은 아일랜드의 유로존에 있습니다.'
        },
        {
          name:'A:',
          speech:'맞아요.'
        },
        {
          name:'B:',
          speech:'그럼, 한 매장만 운영하나요?'
        },
        {
          name:'A:',
          speech:' 네, 더블린 지점입니다. 또 하나 있어요, 안에...'
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
