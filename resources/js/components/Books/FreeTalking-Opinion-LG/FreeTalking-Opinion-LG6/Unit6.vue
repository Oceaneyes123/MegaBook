<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/thai-traditional-street-food-grasshoppers-larvae-market-counter-concept-traditional-exotic-food_169016-4779.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Eat Bugs?
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
      <td class = "lowertable" >Two billion people in the world already eat bugs, and despite the taboo in the developed world, it is a healthy food for humans. In fact, it is impossible to entirely eliminate pest insects in many foods, especially grains. Seeing as nobody has died from this, it is clear that insects can be eaten. In Korea, people eat silkworm pupae or beondegi번데기. In other nations, crickets are milled into flour. Eating bugs may not be considered attractive, but we already do it without knowing, and they offer the nutrients we need for a healthy diet.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Eating insects is something below us. In a TIME Magazine study done on the research of eating insects, once people reached a certain level of economic wealth, they moved on from eating insects. In particular, this study shows that those who were raised eating insects when they were poor ended up not eating them at all afterwards. This proves that humans by nature choose to move on from eating insects. Although eating insects may offer nutrients, the same can be said of healthy fish like salmon and protein rich soy. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>eliminate</b> 제거하다
        </p>
        <p>
          <b>mill</b> (가루가 되도록) 갈다, 으깨다
        </p>
        <p>
          <b>taboo</b> 금기 (사항), 터부
        </p>
        <p>
          <b>consider</b> 사려[고려/숙고]하다
        </p>
        <p>
          <b>nutrients</b> 영양소
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >세계의 20억 명의 사람들이 이미 곤충을 먹으며 선진국에서의 금기에도 불구하고 인간에게는 건강한 음식입니다. 사실, 많은 음식들 특히 곡물에서 해충을 완전히 제거하는 것은 불가능합니다. 아무도 곤충을 먹어서 죽지 않는 것을 보면, 곤충을 먹을 수 있는 것은 분명합니다. 한국에서 사람들은 번데기를 먹습니다. 다른 나라에서는, 귀뚜라미를 밀가루로 으깹니다. 곤충을 먹는 것은 매력적으로 여겨지지 않을지 모르지만, 우리는 인식하지 못한 채 이미 그렇게 하고 있으며, 그것들은 건강한 식단을 위해 우리가 필요로 하는 영양분을 제공합니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >곤충을 먹는 것은 우리와 맞지 않는 일입니다. 곤충을 먹는 것에 대한 연구에 대해서 실시된 타임지의 한 실험에 따르면, 사람들이 특정한 수준의 경제적인 부에 도달하면 그들은 곤충을 먹는 것으로부터 벗어난다고 합니다. 특히, 이 연구는 그들이 가난할 때 곤충을 먹으며 자란 사람들이 후에 그것들을 전혀 먹지 않게 된다는 것을 보여줍니다. 이것은 인간이 본성상 곤충을 먹는 것으로부터 벗어나는 것을 선택한다는 것을 증명합니다. 비록 곤충을 먹는 것이 영양분을 제공할 수 있을지 모르지만, 연어와 같은 건강한 생선과 단백질이 풍부한 콩도 마찬가지입니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you been to a place that serves exotic food? If yes, what was it like? If not, do you plan on visiting one?</li>
          <li>Would you also consider eating a bug? Why or why not?</li>
          <li>What do you think would a bug taste like?</li>
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
