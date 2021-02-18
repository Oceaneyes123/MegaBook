<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://marketplace.canva.com/MADGx9l2kqo/4/screen_2x/canva-woman-at-shoe-store-MADGx9l2kqo.jpg" class = "cover-photo">

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
        padding-bottom: 10px;">Shopping 1 
      </h1>
    </v-layout>
  </v-img>

  <div style=" border-color: #899857; border-style: solid; border-width: 2px;">
  </div>
  <h3  class = "border" >Today's topic</h3>
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



    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Translation</h3>
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

    </div>

    <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #899857; border-style: solid; border-width: 2px;">
    </div>
    <h3 class = "border" style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 0px; background-color: #899857;">Exercise</h3>
    <div style="padding : 16px;">

      <p>
        Fill the gaps with this,that,these,those.
      </p>

      <ol style="margin: 12px;">
        <li>
          Can I try on ( &emsp; &emsp; ) shoes over there?
        </li>
        <li>
          Can I try on ( &emsp; &emsp; ) shoes over there?
        </li>
        <li>
          Can I try on ( &emsp; &emsp; ) shoes over there?
        </li>
        <li>
          Can I try on ( &emsp; &emsp; ) shoes over there?
        </li>
      </ol>

      <p>
        Free response:<br />
        Do you have sales in your country? When are they?<br />
        In your opinion, what are the advantages/disadvantages of shopping in the sales?
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
                    this/these, that/those
                  </p>
                  <p>
                    Things that are very near you, or in your hand:<br />
                    Singular: How much is <b>this</b> shirt?<br />
                    Plural: Are <b>these</b> jeans in the sale?
                  </p>
                  <p>
                    Things that are further from you, that you point at:<br />
                    Singular: I like <b>that</b> mobile phone.<br />
                    Plural: Could I have one of <b>those</b> sandwiches, please?
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
          name:'Assistant:',
          speech:'Do you need any help?'
          },
          {
            name:'Customer:',
            speech:'Yes, how much is this T-shirt? I can’t find the price on it.'
          },
          {
            name:'Assistant:',
            speech:'Er... Let’s have a look... '
          },
          {
            name:'Customer:',
            speech:'Is that it, there?'
          },
          {
            name:'Assistant:',
            speech:'Yes. Thirteen pounds.'
          },
          {
            name:'Customer:',
            speech:'Oh right. OK. Thank you.'
          },
          ],

          seconddialogs:[
          {
            name:'Customer:',
            speech:'Excuse me. I’m just looking at these shoes. I’m a size forty-five, European size. What’s that in a UK size? Do you know?'
          },
          {
            name:'Assistant:',
            speech:'UK size, that’s a ... ten-and-a-half.'
          },
          {
            name:'Customer:',
            speech:'Right. Could I try them in a ten-and-a-half, then, please?'
          },
          {
            name:'Assistant:',
            speech:'Yes, I’ll go and get you a pair.'
          },
          {
            name:'Customer:',
            speech:'Thanks.'
          },
          ],

          thirddialogs:[
          {
            name:'Assistant:',
            speech:'That’s thirty-nine pounds ninety, please.'
          },
          {
            name:'Customer:',
            speech:'Can I pay with this credit card?'
          },
          {
            name:'Assistant:',
            speech:'Yes, we accept those. That’s fine.'
          },
          {
            name:'Customer:',
            speech:'Here you are.'
          },
          {
            name:'Assistant:',
            speech:'Thanks. If you could just sign here. ... Thanks.'
          },
          ],
          
          firsttranslations:[
          {
          name:'점원:',
          speech:'도움이 필요하십니까?'
          },
          {
            name:'고객:',
            speech:'네, 이 티셔츠는 얼마 입니까? 가격을 찾을 수가 없어요.'
          },
          {
            name:'점원:',
            speech:'어... 어디 한번 보죠...'
          },
          {
            name:'고객:',
            speech:'거기에 있나요?'
          },
          {
            name:'점원:',
            speech:'네, 13파운드입니다.'
          },
          {
            name:'고객:',
            speech:'아, 그렇군요. 고마워요.'
          },
          ],

          secondtranslations:[
          {
            name:'고객:',
            speech:'실례합니다만 이 신발을 보고 있어요. 저는 45사이즈, 유럽사이즈입니다. 그건 영국 사이즈로 뭔가요? 아십니까?'
          },
          {
            name:'점원:',
            speech:'영국 사이즈, 그건…10.5입니다.'
          },
          {
            name:'고객:',
            speech:'그렇군요. 그럼 10.5 사이즈 에 한 번 신어 볼 수 있을까요?'
          },
          {
            name:'점원:',
            speech:'네, 제가 가서 한 켤레 가져다 드릴게요.'
          },
          {
            name:'고객:',
            speech:'고마워요'
          },
          ],

          thirdtranslations:[
          {
            name:'점원:',
            speech:'39파운드 90페니 입니다.'
          },
          {
            name:'고객:',
            speech:'이 신용카드로 결제할 수 있을까요?'
          },
          {
            name:'점원:',
            speech:'네, 우리는 그것들을 받습니다. 괜찮아요.'
          },
          {
            name:'고객:',
            speech:'여기 있습니다.'
          },
          {
            name:'점원:',
            speech:'고맙습니다 여기에 서명만 해주면... 고마워요.'
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