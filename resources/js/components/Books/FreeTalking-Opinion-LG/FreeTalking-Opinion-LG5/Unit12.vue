<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/highway-traffic-sunset_1426-1577.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Regulate Car Pollution?
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
      <td class = "lowertable" >The government should regulate cars to address the pollution problem. Because it is convenient for many people to drive to work instead of taking public transportation, many of them are unwilling to stop using their cars. This only adds to the air pollution in big cities like Seoul. It is the government’s job to help make our cities healthier, so they should make laws that limit the number of cars on the roads to reduce pollution. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >The government should not regulate cars. People need their cars to get to work every day. Seoul has a high population density, with more than half the population using public transportation every day. Subway trains and buses are already very crowded during the rush hour. If the government regulates cars, there will be even more people using public transportation. This will put more pressure on Seoul’s aging transportation system, causing delays and accidents.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>pollute</b> 오염시키다
        </p>
        <p>
          <b>reduce</b> 줄이다
        </p>
        <p>
          <b>currently</b> 현재
        </p>
        <p>
          <b>regulate</b> 규제하다
        </p>
        <p>
          <b>convenient</b> 편리한
        </p>
        <p>
          <b>transportation</b> 교통수단
        </p>
        <p>
          <b>population</b> 인구
        </p>
        <p>
          <b>subway</b> 지하철
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >정부는 오염 문제를 고심하기 위해 자동차를 규제해야 합니다. 많은 사람들이 대중 교통을 타는 것 대신에 직장에 운전을 하는 것이 편리하기 때문에 자동차 사용을 사용하지 않는 것을 기꺼이 하려 하지 않을 것입니다. 이것은 서울과 같은 큰 도시에서 공기 오염을 더할 뿐입니다. 우리 도시를 더 건강하게 만드는 것이 정부의 일이기 때문에 오염을 줄이기 위해 도로위의 자동차 대수를 제한하는 법을 만들어야만 합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >정부는 자동차를 규제해선 안됩니다. 사람들은 매일 직장에 가기 위해 자동차가 필요합니다. 서울은 매일 대중교통을 사용하는 사람들의 절반 이상이지만 공기 오염 밀도가 높습니다. 지하철과 버스는 이미 러시아워 동안 매우 붐빕니다. 만약 정부가 자동차를 규제한다면 대중 교통을 이용하는 더 많은 사람들이 있을 것입니다. 이것이 서울의 노화된 교통 시스템에 더 많은 압박을 줘서 지연과 사고의 원인이 됩니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Which do you usually take when going to work? Car or public transportation?</li>
          <li>What do you think are the top contributors of pollution in your country?</li>
          <li>How does the regulation of car usage affect a city’s pollution level?</li>
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
