<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/skyline-architecture-canada-tower-toronto-cn_121-73508.jpg" class="cover-photo">

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
        padding-bottom: 10px;">CN Tower
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">CN Tower</li><br />
      <br />
      <p>
        Jodie and Adam are on vacation in Toronto. They're visiting the CN Tower. But the problem is that Adam doesn’t like heights.<br />
      </p>
      <br />
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
          <u>Make sentences</u><br />
          Example:<br />
            CN Tower/tall   >>  The CN Tower is very tall.<br />
            <br />
            CN Tower/Eiffel Tower, Paris   >>    It’s taller than the Eiffel Tower in Paris.<br />
            <br />
            CN Tower/the world    >>    It’s the tallest tower in the world.<br />
        </p>

        <ol style="margin: 12px;">
          <li>
            <br />
              Mount Everest/high    >>    <br />
              Mount Everest/Mount McKinley    >>    <br />
              Mount Everest/the world     >>    <br />
          </li>
          <li>
            <br />
              Rolls-Royce car/comfortable     >> <br />
              It/Kia    >> <br />
              It/the world     >> <br />
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

        <p>
          Jodie와 Adam은 토론토에서 휴가 중입니다. CN타워를 방문하고 있어요. 하지만 문제는 Adam은 높은 곳을 좋아하지 않는다는 것입니다.<br />
        </p>
        <br />
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
                      비교급 (high > higher) - 두 가지를 비교할 때 사용<br />
                    </li>
                    <li>
                      최상급 (high > the highest) - 세 가지, 혹은 더 많은 것을 비교할 때 사용<br />
                    </li>
                    <li>
                      최상급 구문 : the 최상급 + in + 장소나 범위를 나타내는 단수 명사 (the world, the class, the team등) : ~ 안에서 가장 ~한<br />
                    </li>
                    <li>
                      be on vacation : 휴가중이다<br />
                    </li>
                    <li>
                      33 stories : 33층
                    </li>
                    <li>
                      It's the most exciting place I've ever been to : 내가 갔던 곳들 중에 가장 흥미로운 곳이야
                    </li>
                    <li>
                      It's 100 miles away : 100마일 떨어져 있다
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
          name:'Adam:',
          speech:'Uh, I feel dizzy.'
        },
        {
          name:'Jodie:',
          speech:'The view’s better over here, Adam. You can see farther.'
        },
        {
          name:'Adam:',
          speech:'Don’t go too near the window.'
        },
        {
          name:'Jodie:',
          speech:'Come on! You can see the city better from here.'
        },
        {
          name:'Adam:',
          speech:'Thanks, but I think I will stay here.'
        },
        {
          name:'Jodie:',
          speech:'Can we go up to the space deck? That’s the highest level. It’s 33 stories higher than this one.'
        },
        {
          name:'Adam:',
          speech:'What? Do we have to?'
        },
        {
          name:'Jodie:',
          speech:'It’s the highest public observation gallery in the world. We have to see it.'
        },
        {
          name:'Adam:',
          speech:'Uh… all right.'
        },
        {
          name:'Jodie:',
          speech:'This is fantastic! It’s the most exciting place I’ve ever been to! Think about it, Adam…we’re on the tallest building in the world!'
        },
        {
          name:'Adam:',
          speech:'I am thinking about it.'
        },
        {
          name:'Jodie:',
          speech:'Come over here. This is the best view. You can see Niagara Falls… and it’s 100 miles away.  Oh, sorry. Are you OK?'
        },
        {
          name:'Adam:',
          speech:'Not really. I feel worse!'
        },
        ],

        translations:[
        {
          name:'Adam:',
          speech:'어, 어지러워요.'
        },
        {
          name:'Jodie:',
          speech:'이쪽이 전망이 더 좋아요, Adam. 당신은 더 멀리 볼 수 있습니다.'
        },
        {
          name:'Adam:',
          speech:'창문 가까이 가지 마세요.'
        },
        {
          name:'Jodie:',
          speech:'어서요! 여기서 도시를 더 잘 볼 수 있어요.'
        },
        {
          name:'Adam:',
          speech:'고마워요, 하지만 저는 여기에 머물 것 같아요.'
        },
        {
          name:'Jodie:',
          speech:'우주 갑판으로 올라갈 수 있을까요? 그게 가장 높은 수준이에요. 이것보다 33층 높아요.'
        },
        {
          name:'Adam:',
          speech:'뭐라고요? 꼭 그래야 하나요?'
        },
        {
          name:'Jodie:',
          speech:'그것은 세계에서 가장 높은 대중 관찰 갤러리입니다. 우리는 그것을 봐야 합니다.'
        },
        {
          name:'Adam:',
          speech:'어…알았어요.'
        },
        {
          name:'Jodie:',
          speech:'환상적이에요! 제가 가본 곳 중 가장 신나는 곳이에요! 생각해 보세요, Adam. 우리는 세계에서 가장 높은 빌딩에 있어요!'
        },
        {
          name:'Adam:',
          speech:'저는 그것에 대해 생각하고 있습니다.'
        },
        {
          name:'Jodie:',
          speech:'이리 오세요. 이것이 가장 좋은 풍경입니다. 나이아가라 폭포를 보실 수 있습니다. 100마일 떨어져 있습니다.  아, 죄송합니다. 괜찮아요?'
        },
        {
          name:'Adam:',
          speech:'그렇지 않아요. 기분이 더 안 좋아요!'
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
