<template>

<div :style = "{fontSize: fontSize + 'px'}">

<v-container fluid ma-0 pa-0>

  <v-layout column>
    <v-img
           src="https://marketplace.canva.com/MADGxz0laFQ/4/screen_2x/canva-2-peacock-butterflies-perched-on-yellow-flower-in-close-up-photography-during-daytime-MADGxz0laFQ.jpg">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
      >
        <h1 style="background-color: rgba(13, 13, 13, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Nature</h1>
      </v-layout>
    </v-img>


          <h3 style="background-color: #a7d7c5;   padding-top : 10px;  padding-left : 10px; padding-bottom: 10px;">Reading Practice ( 선생님의 안내에 따라 문장을 읽어 주세요 )</h3>
               <div style="padding : 16px;">

<p>Nature refers to the physical environment around us including the animals and plants. The word "nature"	is derived from the Latin word "natura" which means "essential qualities." Earth, the planet where we live in is the only one known to human knowledge to support life. It has the perfect conditions such as mineral composition and temperature to nurture the natural world as we know it now. From the mountains to the sea, we are enjoying the gifts of Nature so we must take care of it too!
</p>

<h3 style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px;margin-top: 10px; background-color: #a7d7c5;">Vocabulary Review</h3>

<div style="padding : 16px;">



<li style="list-style-type: none;"><u>Physical(adj)</u> - having substance or material existence 육체[신체]의, 물질의
</li>

<li style="list-style-type: none;"><u>Derive(v)</u> -  come from 끌어내다, 얻다
</li>

<li style="list-style-type: none;"><u>Mineral(n)</u> -  solid homogenous inorganic substances occurring in nature having a definite chemical composition 광물; 무기물, 미네랄
</li>

<li style="list-style-type: none;"><u>Composition(n)</u> -  something that is created by arranging several things to form a unified whole 구성 요소들; 구성
</li>

<li style="list-style-type: none;"><u>Nurture(v)</u> - help develop, help grow 육성[양성]하다, 키우다
</li>

<p>Fill in the blanks using the words above.
</p>

<ol style="margin: 12px;">
  <li> _____________ beauty is only temporary.  What is important is the inner beauty.
  </li>

  <li>My mother _________ my abilities and talents.
  </li>

  <li>Diamond is the hardest and most beautiful ____________.
  </li>

  <li>The _______________ of the school population includes students of all ages.
  </li>

  <li>The graduation toga is actually _________ from the clothes of ancient Romans.
  </li>

</ol>

</div>

<h3  style="padding-top: 7px;  margin-left: -18px; margin-right: -18px;  padding-bottom: 10px;  padding-top: 10px; padding-left: 10px; background-color: #a7d7c5; ">Comprehension</h3>
<div style="padding : 16px;">

<ol style="margin: 12px;">
<li>What is nature?
</li>

<li>Where was the term derived from?
</li>

<li>What is so special about the planet Earth?
</li>

<li>How is it able to support life?
</li>
</ol>

</div>

<h3  style="padding-top: 7px;  margin-left: -18px; margin-right: -18px;  padding-bottom: 10px;  padding-top: 10px; padding-left: 10px; background-color: #a7d7c5; ">Translation</h3>
<div style="padding : 16px;">
  <p>자연은 동식물을 포함한 우리 주변의 물리적 환경을 가리킨다. 
     자연이란 말은 본질적인 자질을 뜻하는 라틴어 '나투라(natura)'에서 유래한 말이다. 
     우리가 살고 있는 행성인 지구는 인간의 지식으로 알려진 유일한 생명체다. 
     광물 구성과 온도 등 완벽한 조건을 갖춰 우리가 지금 알고 있는 자연계를 육성한다. 
     산부터 바다까지, 우리는 자연의 선물을 즐기고 있으니 우리도 그것을 돌봐야 해!
  </p>
</div>


<h3  style="padding-top: 7px;  
            margin-left: -18px; 
            margin-right: -18px;  
            padding-bottom: 10px;  
            padding-top: 10px; 
            padding-left: 10px; 
            background-color: #a7d7c5; ">Conversation Samples (선생님과 역할을 나눠서 연습해보세요)</h3>

<div style="padding : 16px;">

<p>
<b>A.</b>
</p>

<table style = "border-collapse: collapse;">

    <tr v-for="dialog in dialogs" :key="dialog">
      <td class = "uppertable" ><b>{{dialog.name}}</b></td>
      <td class = "lowertable" >{{dialog.speech}}</td>
    </tr>

  </table>


<p>
<b>B.</b>
</p>

<table style = "border-collapse: collapse;">

  <tr v-for="dialog2 in dialogs2" :key="dialog2">
    <td class = "uppertable" ><b>{{dialog2.name}}</b></td>
    <td class = "lowertable" >{{dialog2.speech}}</td>
  </tr>

</table>

</div>


<h3  style="padding-top: 7px;  margin-left: -18px; margin-right: -18px;  padding-bottom: 10px;  padding-top: 10px; padding-left: 10px; background-color: #a7d7c5; ">Enhance!</h3>

<div style="padding : 16px;">
<br>

<p>
  The 7 Biomes
</p>

<v-container>
  <v-layout wrap align-content-center>

                        <v-flex xs12 md12 >
                            <v-card hover>

                                <v-card-media src="https://marketplace.canva.com/MADGx71V8qw/4/screen_2x/canva-desert-MADGx71V8qw.jpg">
                                </v-card-media>

                                <v-card-text>
                                    Desert
                                </v-card-text>
                            </v-card>
                        </v-flex>

  </v-layout>
</v-container>

<v-container>
  <v-layout wrap align-content-center>

                        <v-flex xs12 md12 >
                            <v-card hover>

                                <v-card-media src="https://marketplace.canva.com/MADQ5pQSUP4/1/screen/canva-untitled-MADQ5pQSUP4.jpg">
                                </v-card-media>

                                <v-card-text>
                                    Tundra
                                </v-card-text>
                            </v-card>
                        </v-flex>

  </v-layout>
</v-container>

<v-container>
  <v-layout wrap align-content-center>

                        <v-flex xs12 md12 >
                            <v-card hover>

                                <v-card-media src="https://marketplace.canva.com/MADQ5Hfry6Y/1/screen/canva-untitled-MADQ5Hfry6Y.jpg">
                                </v-card-media>

                                <v-card-text>
                                    Savannah
                                </v-card-text>
                            </v-card>
                        </v-flex>

  </v-layout>
</v-container>

<v-container>
  <v-layout wrap align-content-center>

                        <v-flex xs12 md12 >
                            <v-card hover>

                                <v-card-media src="https://marketplace.canva.com/MADGyNyt-jo/4/screen_2x/canva-brown-leaf-trees-on-forest-MADGyNyt-jo.jpg">
                                </v-card-media>

                                <v-card-text>
                                    Deciduous Forest
                                </v-card-text>
                            </v-card>
                        </v-flex>

  </v-layout>
</v-container>

<v-container>
  <v-layout wrap align-content-center>

                        <v-flex xs12 md12 >
                            <v-card hover>

                                <v-card-media src="https://marketplace.canva.com/MADQ4hSZgtg/2/screen_2x/canva-untitled-MADQ4hSZgtg.jpg">
                                </v-card-media>

                                <v-card-text>
                                    Coniferous Forest
                                </v-card-text>
                            </v-card>
                        </v-flex>

  </v-layout>
</v-container>

<v-container>
  <v-layout wrap align-content-center>

                        <v-flex xs12 md12 >
                            <v-card hover>

                                <v-card-media src="https://marketplace.canva.com/MADGv1ldDAc/7/screen_2x/canva-top-view-of-water-falls-MADGv1ldDAc.jpg">
                                </v-card-media>

                                <v-card-text>
                                    Rainforest
                                </v-card-text>
                            </v-card>
                        </v-flex>

  </v-layout>
</v-container>

<v-container>
  <v-layout wrap align-content-center>

                        <v-flex xs12 md12 >
                            <v-card hover>

                                <v-card-media src="https://marketplace.canva.com/MADGyKBOSYo/4/screen_2x/canva-mountain-ranges-covered-in-snow-MADGyKBOSYo.jpg">
                                </v-card-media>

                                <v-card-text>
                                    Mountain
                                </v-card-text>
                            </v-card>
                        </v-flex>

  </v-layout>
</v-container>







</div>



<h3  style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 10px; background-color: #a7d7c5;">You're on the Limelight!</h3>
<div style="padding : 16px;">


<p>Answer the following questions.
</p>

<ol style="margin: 12px;">
  <li>Do you like nature? Why or why not?
  </li>

  <li>What are the ways to enjoy nature?
  </li>

  <li>What is your favorite way? Why?
  </li>

  <li>What natural scenery do you like the most? Why?
  </li>

  <li>What are some natural scenic views in your country?
  </li>

  <li>What natural views in other countries would you like to see? Why?
  </li>

  <li>What is your favorite tree? Why?
  </li>

  <li>What is your favorite animal? Flower? Why?
  </li>

  <li>Would you rather be in a mountain or in a beach? Why?
  </li>

  <li>What are the ways that destroy nature?
  </li>

  <li>What are the effects of destroying the natural environment?
  </li>

</ol>

</div>

<h3  style="padding-top: 7px;  margin-left: -18px; margin-right: -18px; padding-left: 10px; padding-bottom: 10px;  padding-top: 10px; margin-top: 10px; background-color: #a7d7c5;">Translation</h3>
<div style="padding : 16px;">

  <p>
<b>A.</b>
</p>
  <table style = "border-collapse: collapse;">

        <tr v-for="translation in translations" :key="translation">
          <td class = "uppertable" ><b>{{translation.name}}</b></td>
          <td class = "lowertable" >{{translation.speech}}</td>
        </tr>

      </table>

<p>
<b>B.</b>
</p>
      <table style = "border-collapse: collapse;">

        <tr v-for="translation1 in translations1" :key="translation1">
          <td class = "uppertable" ><b>{{translation1.name}}</b></td>
          <td class = "lowertable" >{{translation1.speech}}</td>
        </tr>

      </table>

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
          name:'F :',
          speech:"Can you name the most beautiful natural scenery you have ever seen"
        },
        {
          name:'M :',
          speech:"That is a difficult question! There are so many beautiful natural sights in the world. I have to say the Grand Canyon is one of them!"
        },
        {
          name:'F :',
          speech:"It is found in the US, right?"
        },
        {
          name:'M :',
          speech:"Yes, it is in Arizona. It was so big and beautiful I felt very small when I went there. It was a humbling experience then. How about you?"
        },
        {
          name:'F :',
          speech:"I have to say the Underground River in Palawan!"
        },
        {
          name:'M :',
          speech:"Oh, underground?"
        },
        {
          name:'F :',
          speech:"Yes, it is in the Philippines. There is a 24-km cave there and a river that is 8.2 km long. We went inside by riding a boat and saw many stone formations."
        },
        {
          name:'M :',
          speech:"Nature is so beautiful and wonderful indeed!"
        },
      ],
      dialogs2:[
        {
          name:'F :',
          speech:"Have you heard about the seven biomes of the world?"
        },
        {
          name:'M :',
          speech:"Yes, biome means a major natural community characterized by the dominant forms of plant life and the prevailing climate."
        },
        {
          name:'F :',
          speech:"That is right! The seven forms of biomes are desert, tundra, coniferous forests, deciduous forests, grasslands, mountains and rainforests."
        },
        {
          name:'M :',
          speech:"Correct! However, I'm a bit confused with the coniferous and deciduous forests."
        },
        {
          name:'F :',
          speech:"Coniferous is forest consist mainly of cone-bearing trees such as spruce, hemlock, and fir, which are well suited to the cold climate while deciduous forest is a lively place, where oak, beech, ash, and maple trees are typical, and wildflowers, berries, and many types of insect and animal life abound."
        },
        {
          name:'M :',
          speech:"Oh that's it! Thanks! I think I like rainforest the most though!"
        },
      ],
      translations:[
        {
          name:'F :',
          speech:"지금까지 본 것 중 가장 아름다운 자연 경관을 말할 수 있니?"
        },
        {
          name:'M :',
          speech:"그건 어려운 질문이야! 세상에는 아름다운 자연 경치가 매우 많아. 그랜드 캐년은 그들 중 하나라고 말해야겠어!"
        },
        {
          name:'F :',
          speech:"미국에서 발견된 거 맞지?"
        },
        {
          name:'M :',
          speech:"그래, 애리조나에 있어. 그것은 너무 크고 아름다워서 내가 그곳에 갔을 때 매우 작게 느껴졌어. 그것은 겸허한 경험이었어. 너는?"
        },
        {
          name:'F :',
          speech:"팔라완의 언더그라운드 강이라고 말해야겠어!"
        },
        {
          name:'M :',
          speech:"아, 지하?"
        },
        {
          name:'F :',
          speech:"응, 필리핀에 있어. 그곳에는 24km의 동굴과 8.2km의 강이 있어. 우리는 보트를 타고 안으로 들어가 많은 석조형물을 보았어."
        },
        {
          name:'M :',
          speech:"자연은 정말 아름답고 멋져!"
        },
      ],
       translations1:[
        {
          name:'F :',
          speech:"세계 7대 생물체에 대해 들어본 적 있어?"
        },
         {
          name:'M :',
          speech:"그래, 생물체는 식물 생물의 지배적인 형태와 지배적인 기후로 특징지어지는 주요 자연 공동체를 의미해."
        },
         {
          name:'F :',
          speech:"맞아! 7가지 형태의 생물체는 사막, 툰드라, 침엽수림, 낙엽수림, 초원, 산, 열대우림이다."
        },
         {
          name:'M :',
          speech:"정답! 하지만 침엽수림과 낙엽수림이 좀 헷갈려."
        },
         {
          name:'F :',
          speech:"침엽수림는 주로 가문비나무, 헴록나무, 전나무 등 원추형 나무로 이루어져 있어 추운 기후에 잘 어울리는 반면 낙엽형 숲은 활달한 곳으로 오크나무, 너도밤나무, 물푸레나무, 단풍나무가 대표적이며 야생화, 열매, 여러 종류의 곤충과 동물생물이 풍부해."
        },
         {
          name:'M :',
          speech:"오, 바로 그거야! 고마워! 그래도 나는 열대우림을 가장 좋아하는 것 같아!"
        },
       ],


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

<style lang="css">

p{

  margin-top: 10px;
}

h3{
  padding-top: 7px;

}


body{

  font-size: 16px;
}

</style>
