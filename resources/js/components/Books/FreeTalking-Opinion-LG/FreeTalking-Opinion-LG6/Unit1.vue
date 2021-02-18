<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://images.pexels.com/photos/3184291/pexels-photo-3184291.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should People Be Considered Naturally Good?
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
      <td class = "lowertable" >People are good. When we help others, our bodies naturally react to this charity. In 2013, a study examined the impact of stress and how volunteering could reduce it. They discovered that adults who volunteered for four hours a week were less stressed out. In fact, those volunteers were up to 40% less likely to develop hypertension. In the 1990s, another study examined personal essays written by nuns in the 1930s. Researchers found that the nuns who expressed positive emotions lived about 10 years longer than those who were pessimistic. Being good is actually physically rewarding!</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >People are selfish. The renowned philosopher, Thomas Hobbes argued that people were naturally cruel, greedy and selfish. When we look at the world, is it fair that 10% of the world’s population emits 90% of the world’s greenhouse gases? Is it fair that 71% of the population lives on $10 a day? It isn’t fair, but it is human nature. When one looks into the Darwinian theory of evolution, only the strongest are to survive. In our modern world, the strongest are those with money, and those who are simply born unfortunate must claw to the top.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>unnerve</b> 불안하게 만들다
        </p>
        <p>
          <b>protestor</b> 시위자
        </p>
        <p>
          <b>hypertension</b> 고혈압
        </p>
        <p>
          <b>nun</b> 수녀
        </p>
        <p>
          <b>pessimistic</b> 비관적인
        </p>
        <p>
          <b>physically</b> 육체적으로
        </p>
        <p>
          <b>philosopher</b> 철학자
        </p>
        <p>
          <b>emit</b> (빛, 열, 가스, 소리 등을) 내다
        </p>
         
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >사람들은 선합니다. 우리가 다른 사람들을 도울 때, 우리의 몸은 자연적으로 이 자선적 행위에 반응합니다. 2013년에 한 연구는 스트레스의 영향과 자원봉사가 어떻게 스트레스를 줄일 수 있는지 조사하였습니다. 그들은 일주일에 4시간 자원 봉사한 어른들이 덜 스트레스를 받은 것을 발견하였습니다. 사실, 이 자원 봉사자들은 40%까지 고혈압에 걸릴 확률이 덜 합니다. 1990년대 또 다른 연구는 1930년대 수녀들에 의해 쓰여진 수필을 조사하였습니다. 연구원들은 긍정적인 감정을 표했던 수녀들이 비관적이었던 수녀들보다 약 10년 더 살았음을 발견하였습니다. 선한 것이 사실 육체적으로 보람이 있습니다! </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >사람들은 이기적입니다. 명성 있는 철학가 토마스 홉스는 사람들이 천성적으로 잔인하고, 탐욕적이고 이기적이라고 주장했습니다. 우리가 세상을 볼 때, 세계 인구의 10%가 세계의 온실 가스의 90%를 배출하는 것이 공평할까요? 인구의 71%가 하루에 10달러로 연명하는 것이 공평할까요? 그것은 공평하지 않지만 인간의 천성입니다. 다윈의 진화론을 볼 때 가장 강한 자만이 살아 남습니다. 우리의 현대 세계에서, 가장 강한 자들은 돈을 가진 이들이며, 불행하게 태어난 사람들은 정상까지 이를 악물고 나아갑니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Which do you think is true: man is naturally good, or man is naturally evil? Why?</li>
          <li>What makes a man good?</li>
          <li>Why do you think people do good deeds?</li>
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
