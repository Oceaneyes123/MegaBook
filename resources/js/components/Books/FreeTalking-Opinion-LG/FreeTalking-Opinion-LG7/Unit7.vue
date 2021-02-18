<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/long-hair-guitar-guy-vocalist-duet-singing_23-2148751623.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Solo Singers Versus Groups
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
      <td class = "lowertable" >It is better to be a solo singer than a group member. Although it depends on the contract, groups are usually expected to divide their income. The money they make also partially goes to various companies and staff members. Moreover, solo musicians tend to have more creative control, as group members can clash with each other. In addition, some group members fail to make it big. Who else was in The Jackson 5 besides Michael Jackson? Plus, his fame skyrocketed after leaving the group.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Groups are better than solo singers because of the variety. For instance, Twice has nine members, each with a unique personality and look. Also, the number of NCT members is constantly growing, which is very exciting. There’s always someone new to look forward to. Outside of Korea, there are even bigger groups. The Japanese group AKB48, for example, has more than 130 members! When you get bored of one member, you can always move on to someone else. With solo singers, you’re stuck with just one person.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>income</b> 소득
        </p>
        <p>
          <b>clash</b> 의견 충돌을 일으키다, 언쟁을 벌이다
        </p>
        <p>
          <b>make it big</b> 크게 성공하다
        </p>
        <p>
          <b>skyrocket</b> 급등하다
        </p>
        <p>
          <b>personality</b> 성격
        </p>
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >그룹 멤버보다는 솔로 가수가 되는 것이 좋습니다 계약에 따라 다르지만, 일반적으로 그룹들은 수입을 나눌 것으로 예상됩니다. 그들이 버는 돈은 또한 부분적으로 다양한 회사들과 직원들에게 전달됩니다. 게다가, 솔로 뮤지션들은 그룹 멤버들이 서로 충돌할 수 있기 때문에 더 창의적인 통제력을 갖는 경향이 있습니다. 게다가, 일부 그룹 멤버들은 크게 성공하지 못합니다. 마이클 잭슨 외에 잭슨 5에 누가 더 있었습니까? 게다가, 그의 명성은 그룹을 떠난 후 급상승했습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >그룹이 다양성 차원에서 솔로 가수보다 낫습니다. 예를 들어, 트와이스는 각각 독특한 개성과 외모를 가진 9명의 멤버가 있습니다. 또한 NCT 멤버 수가 지속적으로 증가하고 있어 매우 흥미롭습니다. 항상 기대할 새로운 사람이 있습니다. 한국 바깥에는 더 큰 그룹들이 있습니다. 예를 들어, 일본 그룹 AKB48에는 130 명이 넘는 멤버들이 있습니다! 한 멤버가 지겨워지면 항상 다른 멤버로 넘어갈 수 있어요. 솔로 가수라면 여러분은 한 사람에게만 집중하잖아요.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you usually listen to songs sung by a soloist or a group? Why?</li>
          <li>Do you think it is more advantageous to be a solo singer? Why?</li>
          <li>What do you think is a disadvantage of being in a group than being a soloist?</li>
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
