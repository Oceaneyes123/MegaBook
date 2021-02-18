<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/designer-work-office_158595-1207.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should People Work Four Days A Week?
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
      <td class = "lowertable" >A shorter workweek, specifically a four-day workweek, is ideal because it gives people more time to do other things besides work. For example, people who work four days a week can spend more time with their family and friends. They can also spend their extra time enjoying their hobbies. The workplace can be very stressful, so by spending more time away from work, people can relax and unwind. Then they can go back to work feeling refreshed and energized. Our mental health is extremely important!</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >A four-day workweek is actually quite common for some people in the medical field, including nurses. This might sound great, but the trade-off is that their workdays are long and exhausting. They usually work more than 12 hours a day, with many days lasting up to 14 hours. As a result, many nurses spend their time off sleeping, leaving almost no room for them to spend quality time with their friends and family. Other jobs with short workweeks experience this too, because there is so much work to do.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>specifically</b> 구체적으로 말하면
        </p>
        <p>
          <b>ideal</b> 이상적인
        </p>
        <p>
          <b>unwind</b> 긴장을 풀다
        </p>
        <p>
          <b>trade-off</b> 균형
        </p>
        <p>
          <b>exhausting</b> 친사회적인
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >특히 주4일 근무제처럼 주당 근로 시간이 짧으면 일하는 것 외에도 다른 것들을 할 수 있는 시간이 많아지기 때문에 이상적이다. 예를 들어, 주4일 근무를 하는 사람들은 그들의 가족과 친구들과 더 많은 시간을 보낼 수 있다. 그들은 여가 시간을 취미생활을 즐기며 보낼 수 있다. 근무지에서는 스트레스가 많을 수 있으므로, 일에서 벗어나 더 많은 시간을 보냄으로써 사람들은 긴장을 풀 수 있다. 그리고 나서 그들은 기분이 전환되고 에너지가 가득 찬 느낌으로 직장으로 돌아갈 수 있다. 우리의 정신 건강은 아주 중요하다! </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >주4일 근무제는 간호사를 포함한 의료 분야의 사람들에게 실제로 매우 일반적이다. 멋지게 들릴 수도 있지만, 트레이드 오프는 그들의 근무일이 길고 지치게 한다라는 것이다. 그들은 하루에 12시간 이상을 일하고, 14시간까지 지속되는 여러 날들이 있다. 그 결과 많은 간호사들이 휴가를 수면을 취하는데 쓰고, 그들의 친구들, 가족들과 양질의 시간을 보낼 수 있는 여지를 갖지 못한다. 적은 주당 근무일수를 가진 다른 직업들은 이것을 똑같이 겪고 있다, 왜냐하면 할 일이 아주 많기 때문이다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>How many days do you work in a week?</li>
          <li>In your opinion, what is the most ideal number of days a person should work in a week? Why?</li>
          <li>Do you think implementing a four-day workweek would do more harm than good? Why or why not?</li>
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
