<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/parent-looking-their-children-while-writing-family-text-slate_23-2148208058.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Parents Compare Their Children To Other Children?
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
      <td class = "lowertable" >Parents should be able to compare their children. It is important for a parent to know how well their child is growing up compared to their friends. By looking at other children, parents will know if their children are developing properly. If their child is doing badly in school, but other children are doing well, then maybe their child needs more help. This way, parents can get their child more help and ensure that they do better. It is a parent’s job to make sure that their child will succeed in life.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Parents shouldn’t compare their children. Children are unique individuals, and they need time and space to discover themselves. If a parent is always comparing their son or daughter to other children, that child can feel pressured to become someone that they are not. This can make children very sad and create unnecessary stress for them. It can even ruin a child’s relationships with their parents because they might feel like they are letting down their parents by not being perfect. The worst thing a parent can do is compare their children to others.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>compare</b> 비교하다
        </p>
        <p>
          <b>determine</b> 알아내다, 결정짓다
        </p>
        <p>
          <b>ensure</b> 보장하다, 반드시 ~해주다
        </p>
        <p>
          <b>unique</b> 유일무이한, 독특한
        </p>
        <p>
          <b>discover</b> 발견하다, 알아내다
        </p>
        <p>
          <b>necessary</b> 필수적인
        </p>
        <p>
          <b>unnecessary</b> 불필요한
        </p>
        
      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >부모들은 그들의 아이들을 비교할 수 있어야만 합니다. 부모가 그들의 아이들이 다른 친구들과 비교하여 얼마나 잘 자라고 있는지를 아는 것은 중요합니다. 다른 아이들을 보는 것으로 부모님들은 그들의 아이들이 적절하게 자라고 있는지 없는지를 알 것입니다. 그들의 아이가 학교에서 잘 못하고 있고 다른 아이들은 잘 하고 있다면 아마 그들의 아이는 더 많은 도움이 필요할 것입니다. 이런 식으로 부모들은 그들의 아이가 더 많은 도움을 받고 그들이 더 잘 할 수 있는 것을 확실하게 할 수 있습니다. 그들의 아이가 인생에서 성공하는 것을 확실하게 하는 것이 부모들의 일입니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >부모들은 그들의 아이를 비교해서는 안됩니다. 아이들은 독특한 개인들이고 그들은 자신들을 발견하기 위한 시간과 공간이 필요합니다. 만약 부모가 항상 그들의 아들이나 딸을 다른 아이들과 비교한다면 그 아이는 그들이 아닌 다른 누군가가 되어야 한다는 압박감을 느낄 수 있습니다. 이것은 아이들을 매우 슬프게 만들 수 있고 불필요한 스트레스를 유발합니다. 아이들이 완벽하지 못하는 것으로 부모를 실망시킬 수 있는 것처럼 느낄 수 있어서 그것은 심지어 아이와 부모와의 관계를 망칠 수 있습니다. 부모가 하는 가장 안좋은 일은 그들의 아이를 다른 아이들과 비교하는 것입니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you been compared to other children before? How did it make you feel?</li>
          <li>How do you think does comparison affect a child?</li>
          <li>Would you also compare your children to others? Why or why not?</li>
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
