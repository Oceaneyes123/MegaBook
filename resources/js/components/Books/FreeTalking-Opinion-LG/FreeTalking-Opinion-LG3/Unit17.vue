<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-vector/world-refugee-day-silhouetts_23-2148551263.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should the U.S. Deport Illegal Immigrants?
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
      <td class = "uppertable" ><b>Henry :</b></td>
      <td class = "lowertable" >Illegal immigrants are a threat to U.S. security. According to Peter Gemma, a member of the Constitution Party, around 75 percent of the most-wanted criminals in Los Angeles, Phoenix, and Albuquerque are illegal aliens. He also said, “One quarter of all inmates in California detention centers are Mexican nationals, as are more than 40 percent of all inmates in Arizona and 48 percent in New Mexico jails. Over 53 percent of all burglaries in California, New Mexico, Nevada, Arizona, and Texas are perpetrated by illegal aliens.” </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >It is inhumane to deport undocumented immigrants. They should be offered a chance to gain legal status and eventually earn American citizenship. These immigrants are people, too, and they have families just like everyone else. They are working hard to support their parents, children, and siblings. In addition, the American Jewish Committee stated, “Allowing these immigrants to regularize their status will not only strengthen our national security, but will also stimulate the economy and enhance America’s rich, vibrant, and diverse culture.” </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>inmate</b> 수감자, 재소자
        </p>
        <p>
          <b>burglary</b> 절도(죄)
        </p>
        <p>
          <b>inhumane</b> 비인도적인, 잔혹한
        </p>
        <p>
          <b>undocumented</b> 허가증이 없는
        </p>
        <p>
          <b>stimulate</b> 자극하다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >불법 이민자들은 미국 안보에 위협이 됩니다. 헌법 당원인 피터 젬마 (Peter Gemma)에 따르면 로스앤젤레스, 피닉스, 앨버커키에서 긴급 수배중인 범죄자의 약 75 %가 불법 체류자입니다. 그는 또한 “캘리포니아의 모든 수감자 중 4 분의 1이 멕시코 국적이며, 이들은 애리조나 주에 있는 수감자의 40 % 이상과 뉴멕시코 주 교도소에서 48 %를 차지하고 있습니다. 캘리포니아, 뉴멕시코, 네바다, 애리조나, 그리고 텍사스에서 발생한 강도 사건의 53% 이상이 불법체류자들에 의해 자행되고 있습니다."라고 말했습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >밀입국자를 강제 추방하는 것은 비인도적인 일입니다. 그들은 법적 지위를 얻고 결국 미국 시민권을 얻을 수 있는 기회를 제공해야 합니다 이 이민자들도 역시 사람들이고, 다른 모든 사람들과 마찬가지로 가족도 있습니다. 그들은 부모, 자식, 그리고 형제자매를 지원하기 위해 열심히 일하고 있습니다. 또, 미국 유대교 위원회는 "이 이민자들이 그들의 지위를 합법화 할 수 있도록 하는 것은 우리의 국가 안보를 강화시킬 뿐만 아니라, 경제를 활성화시키고 미국의 풍부하고 활기차고 다양한 문화를 향상시킬 것입니다."라고 말했습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you personally know someone who is an immigrant? Where was he/she from?</li>
          <li>Are you in favor of the U.S. deporting illegal immigrants? If yes, why? If not, then what would you suggest they do instead?</li>
          <li>Which do you think would result in peace? Deporting illegal immigrants or giving them the chance to gain legal status? Why?</li>
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
