<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/small-school-girl-choosing-tablet-book_23-2148764040.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Tablets Replace Textbooks In School?
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
      <td class = "lowertable" >According to several studies, students who own tablets tend to read more books than those who just read regular books. On average, a tablet-owning American student reads 24 books a year on a tablet, but those who don’t have tablets read only 15 books. Furthermore, electronic textbooks on tablets cost less than regular textbooks. According to the Federal Communications Commission, schools in the United States spend more than $8 billion per year on textbooks. Schools can save from $250 to $1,000 per student each year with tablets.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >According to the American Optometric Association, tablets are associated with a variety of health problems, including eyestrain, headaches, blurred vision, and dry eyes. People who use mobile devices, like tablets, are prone to developing musculoskeletal disorders, including carpal tunnel syndrome, neck pain, shoulder pain, and fibromyalgia. Plus, tablets are a threat to the environment. According to The New York Times, using one tablet results in 30 kg of carbon dioxide. Regular books, on the other hand, produce 100 times fewer greenhouse gases. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>publisher</b> 출판사
        </p>
        <p>
          <b>average</b> 평균의
        </p>
        <p>
          <b>furthermore</b> 뿐만 아니라
        </p>
        <p>
          <b>commission</b> 위원회
        </p>
        <p>
          <b>associated</b> 관련된
        </p>
        <p>
          <b>prone</b> (좋지 않은 일을) 하기[당하기] 쉬운
        </p>
        <p>
          <b>greenhouse</b> 온실
        </p>

 

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >몇몇 연구들에 의하면 태블릿을 가진 학생들은 일반적인 책을 읽는 학생들 보다 더 많은 책을 읽는 경향이 있습니다. 평균적으로 태블릿을 소유한 미국 학생 한 명이 태블릿으로 일년에 24권의 책을 읽습니다, 그러나 태블릿을 가지고 있지 않은 학생은 15권만 읽습니다. 더욱이 태블릿 상의 전자책은 일반 교재들 보다 비용이 적게 듭니다. 미국 연방 통신위원회에 따르면 미국의 학교들은 교재에 연간 80억 달러 이상을 지출하고 있습니다. 태블릿을 사용하면 일 년에 학생 한 명당 250불에서 1000불까지 절약할 수 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >미국 검안 협회에 따르면 태블릿은 눈의 피로, 두통, 흐린 시력 및 건조한 눈과 같은 다양한 건강 문제와 관련되어 있습니다. 태블릿과 같은 모바일 장치를 사용하는 사람들은 손목 관절 증후군, 목의 통증, 어깨 통증 및 섬유 근육통을 비롯한 근골격계 질환이 발생하기 쉽습니다. 더욱이 태블릿은 환경에 위협이 됩니다. 뉴욕타임즈에 따르면 태블릿 한 개를 사용하는 것은 30kg의 이산화 탄소를 발생시킨다고 합니다. 반면 일반적인 책들은 100배나 적은 온실 가스를 생산합니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Which learning material would you prefer, tablets or textbooks? Why?</li>
          <li>What do you think are the advantages and disadvantages of tablets over textbooks?</li>
          <li>What do you think would happen if schools no longer use textbooks?</li>
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
