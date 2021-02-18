<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://images04.military.com/sites/default/files/2019-04/ufo-2400.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Do Aliens Exist?
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
      <td class = "lowertable" >We’re not alone! Aliens are real, and even Harry Reid thinks so. He’s an American politician who served as a senator from 1987 to 2017. He’s pushing for more UFO research. He said, “I do believe that the information we have indicates we should do a lot more study. We have hundreds and hundreds of people that have seen the same thing in the sky. It moves a certain way.” He’s familiar with Area 51, too. “I know what they’ve done there,” Reid said.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Aliens do not exist. Researchers from Oxford University say it is highly unlikely that aliens are real. Their study was published in the scientific journal Proceedings of the Royal Society of London. There’s a well-known argument called the Drake equation. It’s been used to show that alien life is possible because of the size of the universe. However, the Oxford researchers debunked it, saying it’s inaccurate and unrealistic. They wrote, “We find a substantial probability of there being no other intelligent life in our observable universe.”</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>politician</b> 정치인
        </p>
        <p>
          <b>debunk</b> 틀렸음을 밝히다
        </p>
        <p>
          <b>inaccurate</b> 오류가 있는
        </p>
        <p>
          <b>probability</b> 개연성
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >우린 혼자가 아닙니다! 외계인은 진짜고, 해리 리드(Harry Reid )도 그렇게 생각해요 그는 1987년부터 2017년까지 상원의원을 지낸 미국 정치인입니다. 그는 UFO 연구를 더 추진하고 있습니다. 그는 "저는 우리가 가진 정보가 우리가 더 많은 연구를 해야 한다는 것을 의미한다고 믿습니다. 우리는 하늘에서 같은 것을 본 수백 명의 사람들이 있습니다. 그것은 특정한 방법으로 움직입니다." “그는 51구역도 잘 알고 있어요 나는 그들이 거기서 무엇을 했는지 알고있습니다."라고 리드가 말했어요. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >외계인이 존재하지 않습니다 옥스포드 대학의 연구원들은 외계인이 진짜일 가능성은 거의 없다고 말합니다. 그들의 연구는 런던 왕립 학회 회보에 실렸습니다. 드레이크 방정식(Drake equation)이라는 잘 알려진 주장이 있습니다. 그것은 우주의 크기 때문에 외계 생명체가 가능하다는 것을 보여주기 위해 사용되었습니다. 하지만, 옥스포드 연구진들은 그것이 부정확하고 비현실적이라고 말하며 그것을 부정했습니다. 그들은 이렇게 썼습니다. "우리는 관찰할 수 있는 우주에는 다른 지적 생명체가 존재하지 않을 상당한 가능성을 발견합니다." </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you believe that aside from humans, other intelligent life forms exist? Why or why not?</li>
          <li>Besides the Earth, do you think another planet that could support life exists?</li>
          <li>Do you think aliens look the same as what they show in movies?</li>
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
