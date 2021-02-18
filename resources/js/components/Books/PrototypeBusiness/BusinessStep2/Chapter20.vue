<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGwNkTy5E/5/screen_2x/canva-photo-of-a-woman-holding-shopping-bags-MADGwNkTy5E.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Shopping 2
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
  Person 1
</p>
      <li style="list-style-type: none;">1. How often does she go shopping for clothes?</li>
      <li style="list-style-type: none;">2. Does she buy much on shopping trips?</li>
      <li style="list-style-type: none;">3. When doesn't she like shopping?</li>

      <p>
        Person 2
      </p>

      <li style="list-style-type: none;">4. Does she like shopping?</li>
      <li style="list-style-type: none;">5. Does she spend a lot of money on clothes?</li>
      <li style="list-style-type: none;">6. Does she buy clothes and never wear them?</li>

      <p>
        Free response:<br />
        Do you prefer shopping alone or with someone?<br />
        Where do you like to go shopping (local shops, big shopping centers, out-of-town stores, markets)?
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
                    Shopping language:<br />
                    free, receipt, size, cash, card, sale, changing
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
          name:'Person 1',
          speech:'I don’t often go shopping for clothes but when I go, I buy quite a lot. I usually know what I want before I go. So I just buy what I need, and come back as soon as I have everything. And I try to go when it’s quiet. I hate shopping when it’s busy.'
        },
        {
          name:'Person 2',
          speech:'I love shopping... especially for clothes. Even if it’s only window shopping. I don’t think I spend too much on clothes. I don’t buy lots of things and then never wear them, like some people. But I can understand why people do that.'
        },
        ],

        translations:[
        {
          name:'Person 1',
          speech:' 나는 옷을 사러 자주 가지 않지만 갈 때는 꽤 많이 산다. 나는 보통 가기 전에 내가 무엇을 원하는지 안다. 그래서 나는 필요한 것만 사고, 모든 것을 갖추는 대로 돌아 온다. 그리고 조용할 때 가려고 노력한다. 나는 바쁠 때 쇼핑하는 것을 싫어한다.'
        },
        {
          name:'Person 2',
          speech:'나는 쇼핑을 좋아한다... 특히 옷의 경우. 윈도우 쇼핑만 해도. 나는 옷에 돈을 많이 쓰는 것 같지 않다. 나는 물건을 많이 사지 않고 다른 사람들처럼 절대 입지 않는다. 하지만 나는 왜 사람들이 그렇게 하는지 이해할 수 있다.'
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
