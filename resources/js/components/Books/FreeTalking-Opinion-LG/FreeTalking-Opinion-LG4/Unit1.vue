<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/high-voltage-post-high-voltage-tower_1127-3215.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Alternative Energy Versus Fossil Fuels
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
      <td class = "lowertable" >Alternative energy can effectively replace fossil fuels. A biofuel is a type of fuel that is produced from biomass, which is plant or animal material. According to the U.S. Department of Energy’s Office of Energy Efficiency and Renewable Energy, “Biofuels can provide a number of environmental advantages over fossil fuels, most notably a reduction in greenhouse gas emissions.” Corn ethanol, for instance, can reduce greenhouse gas emissions by as much as 52 percent over petroleum-based fuels. Biofuels also absorb carbon dioxide from the atmosphere.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Alternative energy isn’t sustainable. We still don’t have the technology to effectively replace fossil fuels with alternative energy. Solar and wind power, for example, aren’t reliable. Jay Leher, a director at the Heartland Institute, said, “The sun’s energy is too widely dispersed, and the land area required to collect it is too vast for solar power to become a large-scale power source.” According to Robert Bradley Jr., CEO of the Institute for Energy Research, wind power is “at its worst when it needs to be at its best.”</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>geothermal</b> 지열의
        </p>
        <p>
          <b>greenhouse</b> 온실
        </p>
        <p>
          <b>emission</b> 배출물
        </p>
        <p>
          <b>sustainable</b> 오랫동안 지속[유지] 가능한
        </p>
        <p>
          <b>disperse</b> (넓은 지역에) 흩어지다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >대체 에너지는 화석 연료를 효과적으로 대체 할 수 있습니다. 바이오 연료는 식물 또는 동물 물질인 바이오 매스에서 생산되는 연료의 한 유형입니다 미국 에너지부의 에너지 효율 및 재생 에너지 사무소에 따르면, "바이오 연료는 화석 연료보다 많은 환경적 이점을 제공할 수 있으며, 특히 온실 가스 배출의 감소이다." 예를 들어 옥수수 에탄올은 석유 기반 연료에 비해 온실 가스 배출물을 52퍼센트까지 줄일 수 있습니다. 바이오 연료는 또한 대기로부터 이산화탄소를 흡수합니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >대체 에너지는 오랫동안 지속 가능하지 않습니다. 화석 연료를 대체 에너지로 효과적으로 대체 할 수 있는 기술이 아직 없습니다. 예를 들어 태양열과 풍력은 신뢰할 수 없습니다. 하트 랜드 연구소의 제이 리어 소장은“태양의 에너지가 너무 넓게 분산되어 있고, 이를 수집하는 데 필요한 토지 면적이 너무 방대해서 태양광이 대규모 전력원이 될 수 없다”고 말했습니다. 에너지 연구소의 CEO 인 로버트 브래들리 주니어에 따르면 풍력은“최상의 상태를 유지해야 할 때 최악의 상태”라고 말합니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What is the main energy source in your country?</li>
          <li>Are you familiar with Alternative energy? What do you think are examples of Alternative energies?</li>
          <li>Do you think it’s ideal to use Alternative energy instead of Fossil fuel?</li>
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
