<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/couple-moving-sofa_23-2147758716.jpg" class="cover-photo">

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
        padding-bottom: 10px;">Moving out
      </h1>
    </v-layout>
  </v-img>

  <hr style="border: 3px solid rgba(32, 64, 81, 1);" width="100%">
  <h3 style="padding-top : 10px;  padding-left : 15px; padding-bottom: 10px;">Dialogue <br /> ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
  <hr width="60%">
  <div style = "padding : 16px;">

      <li style="list-style-type: none;">Moving out</li><br />
      <br />
      <p>
        Travis Smith decided to move out of the city. The city grows bigger every day and there are too many people. He met a real estate agent and talked about buying a farm in the country. Last Saturday the Smiths drove out to see the farm. Mr. Fox, the real estate agent, was standing in front of the farmhouse when they arrived.<br />
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
          <u>Answer</u><br />
        </p>

        <ol style="margin: 12px;">
          <li>
            Where did Smiths go last Saturday?<br />
          </li>
          <li>
            Who was standing in front of the farmhouse when they arrived?<br />
          </li>
          <li>
            Did Travis decide to buy the farm?<br />
          </li>
        </ol>

        <br />
        <p>
          Free response:<br />
          <br />
          Do you think Travis did right when he refused to give Mr. Fox a ride into town?<br />
        </p>


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
          Travis Smith 는 도시를 떠나기로 결심했습니다. 도시는 매일 커지고 사람들은 너무 많습니다. 그는 부동산 중개인을 만나서 시골에서 농장을 사는 것에 대해 이야기했어요. 지난 토요일 Smith  가족은 농장을 보기 위해 차를 몰고 갔습니다. 그들이 도착했을 때 부동산 업자인 Fox 씨가 농가 앞에 서 있었습니다.<br />
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
                      out of : ~로부터
                    </li>
                    <li>
                      grow bigger : ~증가하다, 커지다
                    </li>
                    <li>
                      talk about : ~대해 말하다
                    </li>
                    <li>
                      drive out : 차로 외출하다 
                    </li>
                    <li>
                      in front ot : ~의 앞에
                    </li>
                    <li>
                      a long way from : ~로부터 먼길
                    </li>
                    <li>
                      It's farther than I thought : 내가 생각했던 것보다 더 멀다
                    </li>
                    <li>
                      It’s more peaceful that way : 그것이 더 평화스럽다
                    </li>
                    <li>
                      This farm is much worse than I expected : 이 농장은 내가 기대했던 것보다 훨씬 더 나쁘
                    </li>
                    <li>
                      hope for : 소망하다
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
          name:'Fox:',
          speech:'This is the place. You’re really in the country now.'
        },
        {
          name:'Smith:',
          speech:'It’s a long way from the city. It’s farther than I thought.'
        },
        {
          name:'Fox:',
          speech:'It’s more peaceful that way. Just smell the air. It’s cleaner here than in the city. And the farmhouse is very attractive, don’t you think?'
        },
        {
          name:'Smith:',
          speech:'It’s older and smaller than in the picture. The house needs a paint job and the gate is broken.'
        },
        {
          name:'Fox:',
          speech:'You can fix it, Travis. That will be good exercise for you.'
        },
        {
          name:'Smith:',
          speech:'You said there was a stream, Mr. Fox. Where is it?'
        },
        {
          name:'Fox:',
          speech:'Well, this is the dry season. It isn’t very big this time of year.'
        },
        {
          name:'Smith:',
          speech:'I’m sorry, Mr. Fox. This farm is much worse than I expected. I was hoping for something better and less expensive.'
        },
        {
          name:'Fox:',
          speech:'OK, I give up. Goodbye, Travis. …oh no! I didn’t get enough gas. The tank is empty.'
        },
        {
          name:'Smith:',
          speech:'You can start walking, Mr. Fox.'
        },
        {
          name:'Fox:',
          speech:'Why do you say that, Travis?'
        },
        { 
          name:'Smith:',
          speech:'There’s a dog under the table.Because we’re a long way from town and it’s later than you think. Besides, it’ll be good exercise for you.'
        },
        ],

        translations:[
        {
          name:'Fox:',
          speech:'바로 이곳입니다. 당신은 지금 정말 시골에 있어요.'
        },
        {
          name:'Smith:',
          speech:'도시에서 멀리 떨어져 있어요. 생각보다 멀어요.'
        },
        {
          name:'Fox:',
          speech:'그렇게 하는 것이 더 평화롭습니다. 공기 냄새만 맡아보세요. 여기는 도시보다 깨끗해요. 그리고 그 농가는 매우 매력적이라고 생각하지 않나요?'
        },
        {
          name:'Smith:',
          speech:'그것은 사진보다 더 오래되고 더 작습니다. 집은 페인트칠을 해야 하고 대문이 깨졌어요.'
        },
        {
          name:'Fox:',
          speech:'고칠 수 있어요, 트래비스. 그것은 당신에게 좋은 운동이 될 것입니다.'
        },
        {
          name:'Smith:',
          speech:'냇물이 있다고 했잖아요, Fox 씨. 어디있죠?'
        },
        {
          name:'Fox:',
          speech:'음, 지금이 건기예요. 이 시기에는 별로 크지 않아요.'
        },
        {
          name:'Smith:',
          speech:'죄송합니다, Fox 씨. 이 농장은 내가 예상했던 것보다 훨씬 더 나쁩니다. 저는 더 좋고 덜 비싼 것을 바라고 있었어요.'
        },
        {
          name:'Fox:',
          speech:'좋아요, 저는 포기합니다. 잘 가요, Travis . …이런, 안 돼요! 기름을 충분히 넣지 못했어요. 탱크가 비어 있습니다.'
        },
        {
          name:'Smith:',
          speech:'걷기를 시작할 수 있어요, Fox 씨.'
        },
        {
          name:'Fox:',
          speech:'왜 그렇게 말해요, Travis?'
        },
        {
          name:'Smith:',
          speech:'우리는 마을에서 멀리 떨어져 있고 당신이 생각하는 것보다 더 늦기 때문입니다. 게다가, 그것은 당신에게 좋은 운동이 될 것입니다.'
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
