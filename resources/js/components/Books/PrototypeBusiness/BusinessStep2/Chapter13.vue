<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="//live.staticflickr.com/3180/2926813534_f2be857432_c.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Making plans 2

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
        Are these sentences true (T) or false (F)?
      </p>

      <ol style="margin: 12px;">
        <li>
          It's important to work on the brochure. ( &emsp; )
        </li>
        <li>
          Choosing the photos is quite urgent. ( &emsp; )
        </li>
        <li>
          The website design is a small job. ( &emsp; )
        </li>
        <li>
          Talking about new products is very urgent. ( &emsp; )
        </li>
      </ol>

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
                    first/after/then/next/finally
                  </p>
                  <p>
                    first/after/then/next/finally<br />
                    Then, we can discuss the design.<br />
                    Next, we can talk about the website.<br />
                    After that, let's discuss new products.<br />
                    Finally, we can talk about new products.
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
          name:'Akio:',
          speech:'The most important job is to start work on the sales brochure.'
        },
        {
          name:'Kristi:',
          speech:'Yes, I agree. I think we need to do that first. Um... but then, I think, before we check the prices, we need to choose the photos for the brochure. Hmm... I think that’s more important.'
        },
        {
          name:'Akio:',
          speech:'Yes, you’re right. That is urgent. The marketing people need those photos quickly.'
        },
        {
          name:'Kristi:',
          speech:'Yes. So, I think that...'
        },
        {
          name:'Akio:',
          speech:'And after that we can check the prices.'
        },
        {
          name:'Kristi:',
          speech:'Yes.'
        },
        {
          name:'Akio:',
          speech:'So that’s all we need to do on the brochure. Um...'
        },
        {
          name:'Kristi:',
          speech:'Then. Before we talk about new products, it’s better if we look at the website design, because there’s a lot of work to do on that.'
        },
        {
          name:'Akio:',
          speech:'Hmm. OK. Then, finally, we can talk about new products.'
        },
        {
          name:'Kristi:',
          speech:'Mmm, yes, if we have time. Let’s do that last. It’s less urgent than the other things.'
        },
        {
          name:'Akio:',
          speech:'Yes, OK.'
        },
        {
          name:'Kristi:',
          speech:'So, how much time do we need to do all that?'
        },
        {
          name:'Akio:',
          speech:'Well, if we start quite early and work all day on the…'
        },
        {
          name:'Kristi:',
          speech:'Yes, OK, good idea. Let’s do that.'
        },
        ],

        translations:[
        {
          name:'아키오:',
          speech:'가장 중요한 일은 판매 책자에 대한 작업을 시작하는 것입니다.'
        },
        {
          name:'크리스티:',
          speech:'네, 저도 동의합니다. 우선 그렇게 해야 할 것 같아요. 음... 하지만 가격을 확인하기 전에 책자에 넣을 사진을 골라야 할 것 같아요. 흠... 그게 더 중요한 것 같아요.'
        },
        {
          name:'아키오:',
          speech:'네, 맞습니다. 그것은 긴급한 일입니다. 마케팅 담당자들은 그 사진들을 빨리 필요로 합니다.'
        },
        {
          name:'크리스티:',
          speech:'네, 그래서, 저는...'
        },
        {
          name:'아키오:',
          speech:'그리고 그 후에 우리는 가격을 확인할 수 있습니다.'
        },
        {
          name:'크리스티:',
          speech:'그래요.'
        },
        {
          name:'아키오:',
          speech:'안내 책자에는 그게 전부입니다. 음.. 제가..'
        },
        {
          name:'크리스티:',
          speech:'그럼요. 신제품에 대해 이야기하기 전에 웹사이트 디자인을 살펴보는 것이 좋습니다. 왜냐하면 거기에는 해야 할 일이 많기 때문입니다.'
        },
        {
          name:'아키오:',
          speech:'음.알겠습니다. 그러면 마지막으로 신제품에 대해 이야기 할 수 있습니다.'
        },
        {
          name:'크리스티:',
          speech:'음, 네, 시간이 된다면요. 마지막으로 할게요. 다른 것들보다 덜 급해요.'
        },
        {
          name:'아키오:',
          speech:'네, 알겠습니다.'
        },
        {
          name:'크리스티:',
          speech:'그렇다면, 우리가 그 모든 것을 하기 위해서는 얼마나 많은 시간이 필요할까요?'
        },
        {
          name:'아키오:',
          speech:'음, 만약 우리가 꽤 일찍 시작해서 하루 종일 일을 한다면…'
        },
        {
          name:'크리스티:',
          speech:'네, 좋습니다. 그렇게 하죠.'
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
