<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img
        src="https://image.freepik.com/free-photo/top-view-arrangement-with-crayons_23-2148577671.jpg" style="max-width: 100%; display:block; height: auto;">

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
        padding-bottom: 10px;">Digital Art Versus Traditional Art
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
      <td class = "lowertable" >People need to keep up with our fast-paced society. This means that artists should embrace the latest advancements in technology. Disney, for example, has been focusing on releasing 3D-animated films. Moana, Zootopia, Frozen II, and Toy Story 4 are just a few examples of computer-animated movies produced by Disney. Companies are making 3D films because 3D animation has overtaken traditional 2D animation. Plus, audiences prefer 3D, too. If you want to study animation in college, you should study 3D animation unless you’re okay with being jobless. </td>
    </tr>
    <tr style="color:#1565C0;">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Traditional art is timeless. There’s a reason why art museums exhibit mostly canvas paintings and sculptures made with stone or other materials. Traditional artists put a substantial amount of time and effort into their work. Digital artists, on the other hand, rely on technology to make their creations. There are programs that do all the work for you. All you have to do is make a few mouse clicks. How is this comparable to a traditional sculptor who takes his time to come up with a beautiful masterpiece? </td>
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
          <b>fast-paced</b> 빨리 진행되는  
        </p>
        <p>
          <b>embrace</b> (생각·제의 등을 열렬히) 받아들이다  
        </p>
        <p>
          <b>overtake</b> (수·양·중요도 면에서) 앞지르다[능가 추월하다] 
        </p>
        <p>
          <b>exhibit</b> 전시하다 
        </p>
        <p>
          <b>substantial</b> (양·가치·중요성이) 상당한
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
            <td class = "lowertable" >사람들은 빨리 진행되는 우리의 사회를 따라갈 필요가 있습니다. 이는 예술가들이 최신 기술의 진보를 받아들여야 한다는 것을 의미합니다. 예를 들어, 디즈니는 3D 애니메이션 영화 개봉에 주력해 왔습니다. 모아나, 주토피아, 겨울왕국2, 그리고 토이스토리4는 디즈니가 제작한 컴퓨터 애니메이션 영화의 몇 가지 예일 뿐입니다. 3D 애니메이션이 기존의 2D 애니메이션을 추월했기 때문에 회사들이 3D 영화를 만들고 있습니다. 게다가, 관객들도 3D를 선호합니다. 만약 여러분이 대학에서 애니메이션을 공부하고 싶다면, 여러분이 실직하는 것이 괜찮지 않다면, 3D 애니메이션을 공부해야 합니다. </td>
          </tr>
          <tr style="color:#1565C0;">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >전통 아트는 시대를 초월합니다. 미술관이 주로 캔버스 그림이나 돌이나 다른 재료로 만든 조각품을 전시하는 데는 이유가 있습니다. 전통 예술가들은 그들의 작업에 상당한 시간과 노력을 쏟습니다. 반면에 디지털 예술가들은 자신의 창작물을 만들기 위해 기술에 의존합니다. 모든 일을 하는 프로그램이 있습니다. 마우스를 몇 번 클릭하기만 하면 됩니다. 시간을 들여 아름다운 걸작을 만들어 내는 전통 조각가와 어떻게 견줄 수 있을까요? </td>
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
          <li>Is Digital Art more entertaining than Traditional art? Why or why not?</li>
          <li>Nowadays, people spend most of their time facing their laptop or cellphone screens. With this situation, do you think traditional art is slowly dying?</li>
          <li>How does art relate to life?</li>
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
