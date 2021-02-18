<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/front-view-barista-taking-order_23-2148436222.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Eating out
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color:#402B24; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border white--text" >Today's topic</h3>
  <div style = "padding : 16px;">

    <p>
      1<br />
    </p>
    
    <br />

      <table style = "border-collapse: collapse;">

        <tr v-for="firstdialog in firstdialogs" :key="firstdialog">
          <td class = "uppertable" >{{firstdialog.name}}</td>
          <td class = "lowertable" >{{firstdialog.speech}}</td>
        </tr>
  
      </table>
     
      <br />
     
      <p>
        2<br />
      </p>
      
      <br />

      <table style = "border-collapse: collapse;">

        <tr v-for="seconddialog in seconddialogs" :key="seconddialog">
          <td class = "uppertable" >{{seconddialog.name}}</td>
          <td class = "lowertable" >{{seconddialog.speech}}</td>
        </tr>
  
      </table>


    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border white--text"
        style="padding-top: 7px;
               margin-left: -18px;
               margin-right: -18px;
               padding-left: 10px;
               padding-bottom: 10px;
               padding-top: 10px;
               margin-top: 0px;
               background-color:#402B24;">Translation</h3>
    <div style="padding : 16px;">

      <p>
        1<br />
      </p>
      
      <br />

      <table style = "border-collapse: collapse;">


        <tr v-for="firsttranslation in firsttranslations" :key="firsttranslation">
          <td class = "uppertable" >{{firsttranslation.name}}</td>
          <td class = "lowertable" >{{firsttranslation.speech}}</td>
        </tr>

      </table>
      <br />
      
      <p>
        2<br />
      </p>
      
      <br />


      <table style = "border-collapse: collapse;">


        <tr v-for="secondtranslation in secondtranslations" :key="secondtranslation">
          <td class = "uppertable" >{{secondtranslation.name}}</td>
          <td class = "lowertable" >{{secondtranslation.speech}}</td>
        </tr>

      </table>
    </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color:#402B24; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border white--text" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color:#402B24;">Exercise</h3>
    <div style="padding : 16px;">

      <p>
        Match the pairs to make sentences.
      </p>

      <br />

      <table style = "border-collapse: collapse;">


        <tr v-for="item in items" :key="item">
          <td class = "uppertable" >{{item.name}}</td>
          <td class = "lowertable" >{{item.speech}}</td>
        </tr>

      </table>

      <p>
        Free response:<br />
        Practice ordering a meal in a restaurant.
      </p>

      <v-container grid-list-md text-xs-center>
        <v-layout wrap align-content-center>

          <v-flex xs12 md6 >
            <v-card hover>

              <v-img src="images/menu.jpg" />

            </v-card>
          </v-flex>

        </v-layout>
      </v-container>

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
                    Would you like…?<br />
                    I’d like + noun / I’d like to + verb
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
      firstdialogs:[
          {
          name:'Waiter:',
          speech:'Are you ready to order?'
          },
          {
            name:'Ella:',
            speech:'Yes. For me, um… To start, the tomato soup, please.'
          },
          {
          name:'David:',
          speech:'Yes, the same for me, please. The tomato soup.'
          },
          {
            name:'Waiter:',
            speech:'What would you like for the main course?'
          },
          {
          name:'Ella:',
          speech:'I’d like salmon with rice and peas, please.'
          },
          {
            name:'David:',
            speech:'The lamb, with peas and carrots for me, please. Ivan?'
          },
          {
          name:'Ivan:',
          speech:'I don’t want a starter, just a main course. Can I have steak, chips and peas, please?'
          },
          {
            name:'Waiter:',
            speech:'How would you like the steak?'
          },
          {
          name:'Ivan:',
          speech:'Um… Medium, please.'
          },
          ],

          seconddialogs:[
          {
            name:'Waiter:',
            speech:'Dessert?'
          },
          {
            name:'Ella:',
            speech:'Yes, could I have the apple pie, please.'
          },
          {
            name:'Waiter:',
            speech:'Apple pie.'
          },
          {
            name:'David:',
            speech:'Just a coffee for me, please. Would anyone else like coffee?'
          },
          {
            name:'Ella:',
            speech:'I’ll have one after my dessert.'
          },
          {
            name:'Waiter:',
            speech:'OK. Would anyone else like dessert?'
          },
          ],

          firsttranslations:[
          {
          name:'웨이터:',
          speech:'주문하시겠습니까?'
          },
          {
            name:'엘라:',
            speech:'네. 저는, 음… 우선 토마토 수프부터 부탁해요.'
          },
          {
          name:'데이비드:',
          speech:'그래, 나도 마찬가지야. 토마토 수프 주세요.'
          },
          {
            name:'웨이터:',
            speech:'메인 코스로 뭘 드시겠습니까?'
          },
          {
          name:'엘라:',
          speech:'밥과 완두콩을 곁들인 연어로 부탁해요.'
          },
          {
            name:'데이빗:',
            speech:'완두콩과 당근을 곁들인 양고기를 부탁해요. 이반은?'
          },
          {
          name:'이반:',
          speech:'나는 전채요리가 아니라 그냥 메인 코스를 원해요. 스테이크, 칩, 완두콩을 주시겠습니까?'
          },
          {
            name:'웨이터:',
            speech:'스테이크는 어떻게 하시겠습니까?'
          },
          {
          name:'이반:',
          speech:'음… 미디엄으로 부탁합니다.'
          },
          ],

          secondtranslations:[
          {
            name:'웨이터:',
            speech:'디저트는??'
          },
          {
            name:'엘라:',
            speech:'네, 애플 파이 좀 주시겠습니까?'
          },
          {
            name:'웨이터:',
            speech:'애플파이요.'
          },
          {
            name:'데이비드:',
            speech:'그냥 커피 한 잔만 주세요. 다른 사람 커피 드시겠습니까?'
          },
          {
            name:'엘라:',
            speech:'디저트 먹고 하나 먹을게요.'
          },
          {
            name:'웨이터:',
            speech:'알겠습니다. 디저트 드시겠습니까?'
          },
          ],
        
          items:[
          {
          name:'We have:',
          speech:'for the main course?'
          },
          {
          name:'Are you ready to',
          speech:'for the dessert, please?'
          },
          {
            name:'I’d like soup',
            speech:'order now?.'
          },
          {
          name:'Could I have chicken',
          speech:'anything else to drink?'
          },
          {
            name:'Could I have ice cream',
            speech:'we just have the bill, please?'
          },
          {
          name:'Can I get you',
          speech:'for the starter,'
          },
          {
            name:'No coffee, could',
            speech:'a reservation.'
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
