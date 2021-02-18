<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/children-expressions_23-2148010413.jpg" class="cover-photo">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <h1 style="background-color: rgb(59, 105, 120, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Look, feel, taste, sound, smell
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Look, feel, taste, sound, smell  </li><br />

      <table style = "border-collapse: collapse;">
    
        <tr v-for="dialog in dialogs" :key="dialog">
          <td class = "uppertable" >{{dialog.name}}</td>
          <td class = "lowertable" >{{dialog.speech}}</td>
        </tr>
  
      </table>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;
                                              margin-left: -18px;
                                              margin-right: -18px;
                                              padding-left: 10px;
                                              padding-bottom: 10px;
                                              padding-top: 10px;
                                              margin-top: 0px;
                                              background-color: #204051;">Exercise</h3>
        <div style="padding : 16px;">

        <p>
          <u>Look at the map and fill the blanks. Always answer with a whole sentence.How do these things look, feel, taste, sound or smell to you?</u><br />
              Ex)Fresh coffee smells wonderful. <br />
        </p>

        
        <ol style="margin: 12px;">
          <li>
            cigarette smoke <br />
          </li>
          <li>
            leather seats <br />
          </li>
          <li>
            silk <br />
          </li>
          <li>
            fresh bread <br />
          </li>
          <li>
            freeways <br />
          </li>
          <li>
            stale fish <br />
          </li>
          <li>
            roses <br />
          </li>
          <li>
            old shoes <br />
          </li>
          <li>
            car stereo <br />
          </li>
        </ol>

      </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text" style="padding-top: 7px;
                                              margin-left: -18px;
                                              margin-right: -18px;
                                              padding-left: 10px;
                                              padding-bottom: 10px;
                                              padding-top: 10px;
                                              margin-top: 0px;
                                              background-color: #204051;">Translation</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr v-for="translation in translations" :key="translation">
            <td class = "uppertable" >{{translation.name}}</td>
            <td class = "lowertable" >{{translation.speech}}</td>
          </tr>
  
        </table>
        
</div>
        <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #204051; border-style: solid; border-width: 2px;">
        </div>
        <h3 class = "border white--text" style="padding-top: 7px;
                                                margin-left: -18px;
                                                margin-right: -18px;
                                                padding-left: 10px;
                                                padding-bottom: 10px;
                                                padding-top: 10px;
                                                margin-top: 0px;
                                                background-color: #204051;">Self Study</h3>
        <div style="padding : 16px;">

          <p>

            <v-container grid-list-md text-xs-left>
              <v-layout row wrap>


                <v-flex xs12>
                  <v-card light color="#cae8d5">
                    <v-card-text class="px-10">
                    <li>
                      Notes
                    </li>
                    <ol style="margin: 12px;">
                    <li>
                      감각동사 : look, taste, feel, sound, smell 위에는 형용사가 옵니다.<br />
                        look + 형용사 : ~처럼 보이다 / taste + 형용사 : ~한 맛이 나다<br />
                        feel + 형용사 : ~하게 느껴지다 / sound + 형용사 : ~처럼 들리다 / smell + 형용사 : ~한 맛이 나다 <br />
                        <br />
                        Ex) It doesn't look like a used car : 중고차처럼 보이지 않는다<br />
                          It feels cold in here : 이 안이 춥게 느껴진다<br />
                          they don't taste fresh to me : 나에게는 그것들이 신선한 맛이 나지 않는다<br />
                          it sounds fine to me : 나에게는 괜찮게 들린다<br />
                          it smells wonderful : 멋진 냄새가 난다<br />
                      </li>
                    </ol>
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
          speech:'I like your car, Jackie.'
        },
        {
          name:'B:',
          speech:'Oh, you do? It’s new. I only bought it a week ago.'
        },
        {
          name:'A:',
          speech:'It looks very expensive.'
        },
        {
          name:'B:',
          speech:'Really? I guess new ones are expensive, but this one’s used.'
        },
        {
          name:'A:',
          speech:'It is? It doesn’t look like a used car. It looks brand new.'
        },
        {
          name:'  ',
          speech:'  '
        },
        {
          name:'C:',
          speech:'Brrr! It feels cold in here.'
        },
        {
          name:'D:',
          speech:'It does?'
        },
        {
          name:'C:',
          speech:'Yes, really cold. Is the heat on?'
        },
        {
          name:'D:',
          speech:'Yes, it is. It’ll feel warmer in a minute.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'Waiter!'
        },
        {
          name:'F:',
          speech:'Yes, sir.'
        },
        {
          name:'E:',
          speech:'These vegetables aren’t fresh!'
        },
        {
          name:'F:',
          speech:'But they are fresh, sir..'
        },
        {
          name:'E:',
          speech:'Well, they don’t taste fresh to me. I want you to get the manager.'
        },
        {
          name:'  ',
          speech:'  '
        },
        {
          name:'G:',
          speech:'I’d like you to listen to my new stereo, Eduardo. Does it sound all right?'
        },
        {
          name:'H:',
          speech:'Yes, it sounds fine to me.'
        },
        {
          name:'G:',
          speech:'I think the bass is too loud.'
        },
        {
          name:'H:',
          speech:'No, it sounds perfect. It sounds better than mine.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'I:',
          speech:'Have you changed your perfume?'
        },
        {
          name:'J:',
          speech:'Yes, why? Do you like it?'
        },
        {
          name:'I:',
          speech:'Yes, it smells wonderful. What is it?'
        },
        {
          name:'J:',
          speech:'It’s Roseanne by Devlon..'
        },
        {
          name:'I:',
          speech:'It smells expensive. Is it?'
        },
        {
          name:'J:',
          speech:'I don’t know. It was a present.'
        },
        ],

        translations:[
        {
          name:'A:',
          speech:'Jackie, 당신 차가 마음에 들어요.'
        },
        {
          name:'B:',
          speech:'아, 그래요? 새것이에요. 겨우 일주일 전에 샀어요.'
        },
        {
          name:'A:',
          speech:'아주 비싸 보이네요.'
        },
        {
          name:'B:',
          speech:'정말? 새 것은 비싼 것 같은데, 이건 중고품이에요.'
        },
        {
          name:'A:',
          speech:'그래요? 중고차 같지 않아요. 완전 새것 같아요.'
        },
        {
          name:'  ',
          speech:'  '
        },
        {
          name:'C:',
          speech:'으르렁거려요! 여기는 춥게 느껴져요.'
        },
        {
          name:'D:',
          speech:'그래요?'
        },
        {
          name:'C:',
          speech:'네, 정말 춥습니다. 열이 나나요?'
        },
        {
          name:'D:',
          speech:'네, 그렇습니다. 금방 따뜻해질 거예요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'E:',
          speech:'웨이터요!'
        },
        {
          name:'F:',
          speech:'알겠습니다.'
        },
        {
          name:'E:',
          speech:'이 채소들은 신선하지 않아요!'
        },
        {
          name:'F:',
          speech:'하지만 그것들은 신선합니다.'
        },
        {
          name:'E:',
          speech:'음, 제겐 신선한 맛이 없어요. 당신이 매니저를 구했으면 좋겠어요.'
        },
        {
          name:'  ',
          speech:'  '
        },
        {
          name:'G:',
          speech:'제 새 스테레오인 Eduardo도 좀 들어주세요. 괜찮게 들리나요?'
        },
        {
          name:'H:',
          speech:'네, 괜찮은 것 같아요.'
        },
        {
          name:'G:',
          speech:'베이스 소리가 너무 큰 것 같아요.'
        },
        {
          name:'H:',
          speech:'아뇨, 완벽해 보이네요. 저보다 더 좋은 것 같아요.'
        },
        {
          name:' ',
          speech:' '
        },
        {
          name:'I:',
          speech:'Have you changed your perfume?'
        },
        {
          name:'J:',
          speech:'Yes, why? Do you like it?'
        },
        {
          name:'I:',
          speech:'Yes, it smells wonderful. What is it?'
        },
        {
          name:'J:',
          speech:'It’s Roseanne by Devlon..'
        },
        {
          name:'I:',
          speech:'It smells expensive. Is it?'
        },
        {
          name:'J:',
          speech:'I don’t know. It was a present.'
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
  border-color: transparent #204051 transparent transparent;
  position: absolute;
  top: 0px;
  margin-left: 190px;
}
.border {
  position: relative;
  left: 0px;
  width: 200px;
  height: 40px;
  background: #204051;
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
