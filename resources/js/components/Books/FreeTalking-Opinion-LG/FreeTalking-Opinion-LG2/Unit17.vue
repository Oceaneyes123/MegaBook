<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/overhead-aerial-drone-shot-different-sized-boats-docked-close-each-other-near-pier_181624-9211.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >
        <transition name="slide-fade">
        <h1 v-if="showTitle" style="background-color: rgb(139, 84, 63, 0.7);
        width: 100%;
        padding-top : 10px;
        padding-left : 10px;
        padding-bottom: 10px;">Amusement Parks Versus Beaches
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div style=" border-color: #2F4674; border-style: solid; border-width: 2px;">
  </div>

  <h3  class = "border white--text" style = "border-radius: 0px 0px 70px 0px;" >Topic</h3>
  <div style = "padding : 16px; line-height: 1.6;">

    <table style = "border-collapse: collapse;">

    <tr>
      <td class = "uppertable" ><b>Henry :</b></td>
      <td class = "lowertable" >Amusement parks are obviously better. They feature a variety of attractions, so it’s almost impossible to run out of things to do! For example, Lotte World has an ice skating rink, carousels, roller coasters, and many other rides. It is also chock full of restaurants and food stands, making it possible to satisfy everyone’s tastes. Beaches, on the other hand, serve a specific purpose. They are perfect for people who want to swim or play in the sand but are not ideal for those who loathe the sun. </td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >The beach is the best place to go on a vacation during the summer. In the spring, fall, and winter, it is too chilly to visit the beach. Take advantage of the summer weather, which is nice and hot, and visit the beach! Since amusement parks are open all year round, make the wise decision to visit the beach during the summer. In addition, beaches are great because you can spend quality time with your family. You can get even closer to your family by collecting seashells together. </td>
    </tr>

    </table>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #2F4674; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text"
          style="border-radius: 0px 0px 70px 0px;
                 padding-top: 7px;
                 margin-left: -18px;
                 margin-right: -18px;
                 padding-left: 10px;
                 padding-bottom: 10px;
                 padding-top: 0px;
                 margin-top: 0px;">Vocabulary</h3>
      <div style="padding : 16px;">

        <p>
          <b>carousel</b> 회전목마  
        </p>
        <p>
          <b>chock-full</b> 꽉 들어찬  
        </p>
        <p>
          <b>satisfy</b> 만족시키다  
        </p>
        <p>
          <b>taste</b> 입맛 
        </p>
        <p>
          <b>ideal</b> 이상적인 
        </p>
        <p>
          <b>loathe</b> 혐오하다 
        </p>
        <p>
          <b>take advantage of</b> ~을 이용하다, ~을 기회로 활용하다 
        </p>
        <p>
          <b>quality</b> 훌륭한 
        </p>

      </div>

      <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #2F4674; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text"
          style="border-radius: 0px 0px 70px 0px;
                 padding-top: 7px;
                 margin-left: -18px;
                 margin-right: -18px;
                 padding-left: 10px;
                 padding-bottom: 10px;
                 padding-top: 0px;              
                 margin-top: 0px;
                 width: 100px;">해석</h3>
      <div style="padding : 16px;">

        <table style = "border-collapse: collapse;">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >놀이공원이 확실히 더 낫습니다. 다양한 놀이기구를 제공하므로 할 일이 바닥나는 것은 거의 불가능해요! 예를 들어, 롯데 월드에는 아이스 링크, 회전 목마, 롤러 코스터 및 기타 많은 놀이기구가 있습니다. 또한 식당과 음식 가판대가 꽉 들어 차 있어 모두의 입맛을 만족시킬 수 있습니다. 반면에, 해변은 특정한 목적을 제공합니다. 그것들은 모래에서 수영하거나 놀고 싶은 사람들에게는 완벽하지만 태양을 혐오하는 사람들에게는 이상적이지 않습니다.</td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >당근, 시금치, 버섯, 양배추 같은 야채는 요리되면 더 많은 항산화제를 제공해. 요리로 인한 열은 야채의 세포벽을 부수는데 도움이 된다. 이것은 신체가 더 많은 영양분을 섭취하도록 도와줘.해변은 여름에 휴가를 갈 수 있는 최고의 장소입니다. 봄, 가을, 겨울에는, 해변을 방문하기엔 너무 쌀쌀합니다. 멋지고 더운 여름 날씨를 이용하고 해변을 방문하십시오! 놀이공원은 일년 내내 열려 있기 때문에, 여름에 해변을 방문하는 현명한 결정을 하세요. 게다가, 해변은 가족과 함께 좋은 시간을 보낼 수 있기 때문에 좋습니다. 조개 껍질을 함께 모으면 가족과 더욱 가까워질 수 있습니다.</td>
          </tr>
      
          </table>


      </div>

     <div style="margin-left: -18px; margin-right: -18px; margin-top: 10px; border-color: #2F4674; border-style: solid; border-width: 2px;">
      </div>
      <h3 class = "border white--text"
          style="border-radius: 0px 0px 70px 0px;
                 padding-top: 7px;
                 margin-left: -18px;
                 margin-right: -18px;
                 padding-left: 10px;
                 padding-bottom: 10px;
                 padding-top: 5px;
                 margin-top: 0px;">Questions</h3>
      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you like going to amusement parks? If yes, who do you like going with?</li>
          <li>When is the best time to visit the beach?</li>
          <li>How do you make your amusement park or beach visits memorable?</li>
        </ol>

    
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
      showTitle:false


    }

  },

mounted(){
  this.showTitle=true
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


.border {
  position: relative;
  left: 0px;
  width: 255px;
  height: 40px;
  background: #2F4674;
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
  width: 0%;
  white-space: nowrap;
}

.lowertable {
border: 0px solid #dddddd;
text-align: left;
padding: 8px;
}

.normaltext {
  font-weight: normal;
}

.replace {
  counter-reset: list;
}
.replace > li {
  list-style: none;
  position: relative;
}
.replace > li:before {
  content: counter(list, upper-alpha) ":";
  counter-increment: list;
  position: absolute;
  left: -1.4em;
}

.slide-fade-enter-active {
  transition: all 3s ease;
}
.slide-fade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active below version 2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
}


</style>
