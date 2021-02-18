<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://images.pexels.com/photos/1632788/pexels-photo-1632788.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Replace Traditional Buildings With Modern Ones?
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
      <td class = "lowertable" >Tradition is important. When the Japanese Emperor instituted the Meiji Reform and modernized Japan, he had to face a revolution to realize that he needed to compromise with his country’s culture. In Korea, when the hanok houses were bulldozed by President Park Chung-hee, a lot of Korean culture was sacrificed in the name of change. The Japanese have an excellent blend of culture and modern technology, and enthusiastic tourists average to 24 million a year. In comparison, hanok homes could have been a part of the cultural attractions of the nation, but have been removed.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Tradition should not impede on progress. In New York City, Harlem was the most violent neighborhood until its sudden shift to modernization. Within 20 years, serious crime dropped by 71% and the neighborhood went through many positive changes. Although many argue that the buildings demolished were a part of New York City’s historic Harlem renaissance, it was clear that the neighborhood was suffering. Gentrification and modernization saved it. If it were not for these changes, the neighborhood would most likely have descended into crime and decay.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">
        <p>
          <b>demolish</b> (건물을) 철거하다
        </p>
        <p>
          <b>face</b> (상황에) 직면하다
        </p>
        <p>
          <b>bulldoze</b> 불도저로 밀다
        </p>
        <p>
          <b>sacrifice</b> 희생, 희생물
        </p>
        <p>
          <b>blend</b> 섞다
        </p>
        <p>
          <b>enthusiastic</b> 열렬한, 열광적인
        </p>
        <p>
          <b>impede</b> (진행을) 지연시키다
        </p>
        <p>
          <b>descend</b> 내려오다
        </p>
        <p>
          <b>decay</b> (진행을) 부패
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >전통은 중요합니다. 일본의 황제가 메이지 개혁을 도입하고 일본을 현대화했을 때, 그는 그가 나라의 문화와 타협을 할 필요를 실현하기 위해 혁명에 직면해야 했습니다. 한국에서, 한옥집이 박정희 대통령에 의해 불도조로 밀어졌을 때, 한국 문화의 많은 부분이 변화라는 이름 아래 희생되었습니다. 일본인들은 문화와 현대 기술을 훌륭하게 조합시켰으며, 열정적인 관광객들은 평균 매년 2천400만명에 달합니다. 비교해 보면, 한옥집은 이 나라의 문화적인 명소의 일부분이었지만 제거되어 왔습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >전통은 진보를 막으면 안 됩니다. 뉴욕 시티의 할렘은 현대화로의 갑작스러운 변화가 있기까지 가장 폭력적인 지역이었습니다. 20년 이내, 심각한 범죄는 71% 감소하였고, 이 지역은 많은 긍정적인 변화를 겪었습니다. 비록 많은 이들이 철거된 건물들이 뉴욕 시티의 역사적인 할렘 르네상스의 일부분이라고 주장하지만, 이 지역이 고통을 겪고 있었다는 것은 분명합니다. 고급주택화와 현대화가 이를 살렸습니다. 이러한 변화들이 아니었더라면, 이 지역은 범죄와 부패로 타락했었을 것입니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Why is tradition important?</li>
          <li>Which architectural structures do you like more? Traditional, modern and futuristic, or a mix of both? Why?</li>
          <li>Do you think tradition plays an important role in a country’s progress?</li>
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
