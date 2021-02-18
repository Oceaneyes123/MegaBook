<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/hey-what-is-there-cute-little-boy-drives-his-first-car_1304-2719.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Korea Lower Its Driving Age?
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
      <td class = "lowertable" >You must be 18 years old to obtain a regular driver’s license in Korea. This makes it very inconvenient for many teenagers. At 16, American students can already drive to school, pick up their friends, and take their family to various destinations. Korean teenagers should have this liberty as well. If Americans can drive at the age of 16, why can’t Koreans? Canada, Colombia, and several other countries allow 16-year-olds to drive as well, and these countries don’t have more instances of traffic accidents. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Last year, the Australian state of Victoria rejected the proposition to lower the minimum driving age from 18 to 17. Why? Well, it was decided that lowering the limit would result in more fatal accidents. According to the National Highway Traffic Safety Administration, there are about 2,000 fatalities every year among teenage drivers in the U.S. There are studies that show that teenagers are more prone to make risky decisions while driving. They also have the lowest rate of seatbelt use compared with other age groups.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>grant</b> 허가하다
        </p>
        <p>
          <b>follow suit</b> ~에 따르다
        </p>
        <p>
          <b>obtain</b> 얻다
        </p>
        <p>
          <b>destination</b> 목적지
        </p>
        <p>
          <b>liberty</b> 자유
        </p>
        <p>
          <b>instance</b> 사례
        </p>
        <p>
          <b>proposition</b> 법률 개정안
        </p>
        <p>
          <b>fatal</b> 치명적인
        </p>
        <p>
          <b>fatality</b> 치사율
        </p>
        <p>
          <b>prone to</b> ~을 잘하는
        </p>
        <p>
          <b>seatbelt</b> 안전벨트
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >한국에서 보통의 운전면허증을 받으려면 18살이 되어야 합니다. 이것은 많은 십대들을 매우 불편하게 만듭니다. 16살에 미국 학생들은 이미 학교에 운전해서 가고, 친구들을 태워주고, 그들의 가족을 다양한 목적지로 데려다 줄 수 있습니다. 한국의 십대들도 역시 이 자유를 가져야 합니다. 미국인들이 16살에 운전할 수 있다면 한국인은 왜 안되나요? 캐나다, 콜롬비아, 그리고 몇몇 다른 국가들 역시 16살이 운전할 수 있도록 허락합니다. 그리고 이 나라들은 더 많은 교통사고 사례를 가지고 있지 않습니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >작년에 호주의 빅토리아주는 운전 가능한 최소 연령을 18세에서 17세로 낮추자는 제안을 거절했습니다. 왜 그랬을까요? 글쎄요, 그것은 제한을 낮추는 것이 더 치명적인 사고를 초래한다고 결정되었기 때문입니다. 국도 교통 안전청에 따르면 미국의 십대 운전자 중에 매년 2천명의 사망자가 발생합니다. 10대들이 운전 중에 위험한 결정을 내리는 경향이 있음을 보여주는 연구가 있습니다. 그들은 또한 다른 연령 집단에 비해 안전 벨트 사용률이 가장 낮습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you have a driver’s license? How old were you when you got your driver’s license??</li>
          <li>Are you in favor of lowering the driving age? Why or why not?</li>
          <li>Do you think teenagers below eighteen are responsible enough to drive and have a driver’s license? Why or why not?</li>
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
