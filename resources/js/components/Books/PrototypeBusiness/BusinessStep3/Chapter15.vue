<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADQ4xUstzE/1/screen/canva-road-in-san-fransisco-MADQ4xUstzE.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Sightseeing
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


      <br />
      <p>
      3<br />
      </p>
      <br />

        
      <table style = "border-collapse: collapse;">

        <tr v-for="thirddialog in thirddialogs" :key="thirddialog">
          <td class = "uppertable" >{{thirddialog.name}}</td>
          <td class = "lowertable" >{{thirddialog.speech}}</td>
        </tr>
  
      </table>

      <br />
      <p>
      4<br />
      </p>
      <br />

        
      <table style = "border-collapse: collapse;">

        <tr v-for="fourthdialog in fourthdialogs" :key="fourthdialog">
          <td class = "uppertable" >{{fourthdialog.name}}</td>
          <td class = "lowertable" >{{fourthdialog.speech}}</td>
        </tr>
  
      </table>


<div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #402B24; border-style: solid; border-width: 2px;">
</div>
<h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #402B24;">Exercise</h3>
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


  <br />
  <p>
  3<br />
  </p>
  <br />


  <table style = "border-collapse: collapse;">


    <tr v-for="thirdtranslation in thirdtranslations" :key="thirdtranslation">
      <td class = "uppertable" >{{thirdtranslation.name}}</td>
      <td class = "lowertable" >{{thirdtranslation.speech}}</td>
    </tr>

  </table>

  <br />
  <p>
  4<br />
  </p>
  <br />


  <table style = "border-collapse: collapse;">


    <tr v-for="fourthtranslation in fourthtranslations" :key="fourthtranslation">
      <td class = "uppertable" >{{fourthranslation.name}}</td>
      <td class = "lowertable" >{{fourthtranslation.speech}}</td>
    </tr>

  </table>

   
      <p>
        Free response:<br />
        Talk about tourism in your town/region
      </p>
      <p>
        What are the most interesting places to visit?<br />
        What’s available for tourists at the places(guided tours, souvenirs…)?
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
                  Useful language
                </p>
                <p>
                  Excuse me? Is there a tourist information office near here?<br />
                  Do you have any information/booklets/leaflets about the history of the island?<br />
                  Do you have any maps of the city centre?<br />
                  You can visit the museum with a guide. There’s a guided tour every hour.
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
          name:'A:',
          speech:'Hi.'
          },
          {
            name:'B:',
            speech:'Hello. Do you have any information about Alcatraz? Any… booklets or leaflets?'
          },
          {
            name:'A:',
            speech:'Yes. Just behind you, on the shelf, there.'
          },
          {
            name:'B:',
            speech:'Ah, OK. Thank you.'
          },
          ],

          seconddialogs:[
          {
            name:'A:',
            speech:'Hi.'
          },
          {
            name:'B:',
            speech:'Hi. Is there anywhere near here where you can buy gifts… and souvenirs?'
          },
          {
            name:'A:',
            speech:'Yeah. If you turn right out of the door, then take the first right, there are gift shops all along the … the street, there.'
          },
          {
            name:'B:',
            speech:'OK. Thanks very much.'
          },
          ],

          thirddialogs:[
          {
            name:'B:',
            speech:'Can you visit the museum all day? What are the opening times?'
          },
          {
            name:'A:',
            speech:'It opens at ten and closes at five. If you want to take a guided tour, they start every hour, on the hour and last… I think they last forty-five minutes, but I’ll just check…'
          },
          ],

          fourthdialogs:[
          {
            name:'B:',
            speech:'Excuse me. Have you got any street maps?'
          },
          {
            name:'A:',
            speech:'Sure.'
          },
          {
            name:'B:',
            speech:'....Thanks. How much are they?'
          },
          {
            name:'A:',
            speech:'They’re free.'
          },
          ],
          
          firsttranslations:[
          {
          name:'A:',
          speech:'안녕하세요.'
          },
          {
            name:'B:',
            speech:'안녕하세요. 알카트라즈에 대해 아는 거 있어요? 책자나 전단지는요?'
          },
          {
            name:'A:',
            speech:'네. 바로 뒤에, 선반 위에, 저기요.'
          },
          {
            name:'B:',
            speech:'아, 알았어요. 감사합니다.'
          },
          ],

          secondtranslations:[
          {
            name:'A:',
            speech:'안녕하세요.'
          },
          {
            name:'B:',
            speech:'안녕하세요. 이 근처에 선물과 기념품을 살 수 있는 곳이 있나요?'
          },
          {
            name:'A:',
            speech:'네. 만약 당신이 문에서 오른쪽으로 돌면, 저기 길가에 선물 가게들이 있어요.'
          },
          {
            name:'B:',
            speech:'알겠습니다. 정말 고마워요.'
          },
          ],

          thirdtranslations:[
          {
            name:'B:',
            speech:'박물관은 하루 종일 하나요? 몇 시부터 몇 시까지입니까?'
          },
          {
            name:'A:',
            speech:'10시에 열고 5시에 닫아요. 가이드 투어를 하고 싶다면,그들은 매시간, 그리고 마지막에 시작한해요. 45분정도 지속되는것 같은데, 그냥 확인해 볼게요.'
          },
          ],

          fourthtranslations:[
          {
            name:'B:',
            speech:'실례합니다만. 거리 지도는 가지고 계신가요?'
          },
          {
            name:'A:',
            speech:'물론입니다.'
          },
          {
            name:'B:',
            speech:'……고마워. 그것은 얼마입니까?'
          },
          {
            name:'A:',
            speech:'무료입니다.'
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
