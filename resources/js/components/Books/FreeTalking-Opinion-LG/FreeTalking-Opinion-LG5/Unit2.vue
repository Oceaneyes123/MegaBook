<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/close-up-hand-holding-phone-front-laptop_23-2148295800.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should The Internet Be Free?
      </h1>
      </transition>
    </v-layout>
  </v-img>

  <div class = "line-top-lg">
  </div>
  <h3  class = "lower-header-lg white--text">Topic</h3>

  <div style = "padding : 16px; line-height: 1.6;">

    <table class = "standard-table">

    <tr>
      <td class = "uppertable" ><b>David :</b></td>
      <td class = "lowertable" >Mark Zuckerberg, the CEO and founder of Facebook, believes that basic internet service should be free for everyone across the globe. He says that it won’t be too difficult. “Almost 90 percent of the world’s population already lives within range of an existing cellular network,” Zuckerberg says. “For everyone in those areas, we don’t need to build completely new kinds of infrastructure to help them connect. We just need to show why it’s valuable and make it affordable.” He even has an organization dedicated to making the internet free for everyone. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >It costs a lot of money to run and maintain the hardware that makes the internet possible. If we make the internet free of charge, then who’s going to pay to run it? Money doesn’t just come out of thin air, you know. Obviously, taxpayers - that’s us - will have to pick up the cost so that we can have “free” internet. I guess Henry thinks that it’s unfair how some people can’t go on the internet and browse Facebook or read webtoons. Can’t people just read books or something?</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>founder</b> 창립자
        </p>
        <p>
          <b>infrastructure</b> 기반 시설
        </p>
        <p>
          <b>affordable</b> 가격이 알맞은
        </p>
        <p>
          <b>organization</b> 기구
        </p>
        <p>
          <b>dedicate</b> 전념하다
        </p>
        <p>
          <b>maintain</b> 유지하다
        </p>
        <p>
          <b>hardware</b> 장비
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >페이스북의 최고경영자이자 창립자인 마크 저커버그는 기본적인 인터넷 서비스가 전세계에 있는 모든 사람들에게 무료화되어야 한다고 생각합니다. 그는 그것이 너무 어렵지 않을 것이라고 말합니다. “전 세계 인구의 거의 90퍼센트가 이미 존재하는 셀룰러 네트워크 범위 내에 살고 있습니다.”라고 저커버그가 말합니다. “그 지역의 모든 사람들을 위해 그들의 연결을 돕는 완전히 새로운 종류의 기반 시설을 만들 필요가 없습니다. 우리는 단지 왜 그것이 가치 있는지를 보여주고 그것을 저렴하게 만들 필요가 있습니다. 그는 심지어 누구나 인터넷을 무료로 사용할 수 있게 만드는 조직을 가지고 있습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >인터넷이 가능하게 만드는 장비를 운영하고 유지하려면 많은 비용이 듭니다. 우리가 인터넷 비용을 무료화 하면 누가 그것을 운영하기 위해 돈을 내겠습니까? 돈은 아시다시피 허공에서 나오는 것이 아닙니다. 명백히 우리 납세자들은 “무료”인터넷을 사용하기 위해 비용을 내야 할 것입니다. 저는 헨리가 어떤 사람들이 인터넷에 접속해서 페이스북을 보거나 웹툰을 읽을 수 없는 것이 불공평하다고 생각한다고 추측합니다. 사람들은 그냥 책을 읽거나 다른 것을 하면 안되나요? </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Is the internet important to you? If yes, how so?</li>
          <li>Why do you think we need to pay for the internet?</li>
          <li>Do you agree that the internet should be free? Why or why not?</li>
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

</style>
