<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/teenager-having-fun-skatepark_23-2148758471.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should skateboarding, biking, and skating be banned in public places?
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
      <td class = "lowertable" >Skateboarding, biking, and skating should be banned in public places. People enjoy them at different ability levels. Beginners often lose control, and even those who are advanced can make mistakes. They may hurt themselves and others if they crash. Secondly, more people are using bikes as a primary form of transportation. Some people ride their bikes to work every morning. Bikers are starting to get in the way of cars!</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Skateboarding, biking, and roller skating should not be banned in public places. These are popular activities. People not only enjoy doing them, but they are also great forms of exercise. If we ban them in public places, then people will do them less. Furthermore, people need open spaces to bike, skateboard, and roller skate. If these activities are banned in public spaces, where will people do them?</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>ability</b> 능력
        </p>
        <p>
          <b>lose control</b> 제어할 수 없게 되다
        </p>
        <p>
          <b>advanced</b> 숙련된
        </p>
        <p>
          <b>crash</b> 부딪히다
        </p>
        <p>
          <b>primary</b> 주요한
        </p>
        <p>
          <b>get in the way</b> 방해하다
        </p>
       </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >스케이트 보드, 자전거, 스케이트를 공공 장소에서 금지해야 합니다. 사람들은 그것들을 다양한 능력 수준에서 즐깁니다. 초보자들은 종종 자제력을 잃고, 심지어 숙련자들도 실수를 할 수 있습니다. 부딪힐 경우 그들은 자신과 타인을 다치게 할 수 있습니다. 다음으로, 더 많은 사람들이 교통 수단의 주요 형태로 자전거를 이용하고 있습니다. 어떤 사람들은 매일 아침 직장에 자전거를 타고 출근합니다. 자전거는 자동차를 방해하기 시작했습니다!</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >스케이트 보드, 자전거, 스케이트를 공공 장소에서 금지하면 안 됩니다. 이것들은 인기 있는 활동입니다. 그것은 사람들이 즐길 뿐만 아니라, 아주 좋은 운동의 형태입니다. 만약 우리가 그것을 공공 장소에서 금지한다면, 사람들은 그것을 덜 하게 될 것입니다. 게다가, 사람들은 자전거와 보드, 스케이트를 타기 위해 야외 장소가 필요합니다. 만약 이러한 활동이 공공 장소에서 금지된다면, 사람들은 그것을 어디에서 해야 하나요?</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you ever tried skateboarding, biking, or skating? If no, which one would you like to try and why?</li>
          <li>Do you think such activities are dangerous and shouldn’t be done in public places? Why?</li>
          <li>Does your city have facilities to enjoy these activities?</li>
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
