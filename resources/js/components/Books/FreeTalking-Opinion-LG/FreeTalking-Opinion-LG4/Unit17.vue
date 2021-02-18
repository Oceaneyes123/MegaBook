<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/girl-holding-glass-apple-slices-looking-ring-tailed-lemur-zoo_23-2147924056.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Is It Okay To Have Zoos?
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
      <td class = "lowertable" >Zoos play a critical role in educating people about the different types of animals on Earth. These days, zoos try to raise awareness about various environmental problems and stress the importance of conservation. Zoo workers often visit schools to make presentations. In addition, many students visit zoos to broaden their knowledge about endangered species. They can also learn more about animals in general without having to travel to distant places. Moreover, zoos serve as havens for many animals, especially those that are often hunted for their fur or ivory.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Since they’re trapped in tight enclosures, zoo animals suffer from immense stress. Locking them up takes away their freedom, and animals that are born in zoos never get to experience the outside world. And if they get released in the wild, it’s difficult for them to adjust to their new surroundings. They tend to get ostracized by their own kind, becoming outcasts in what is supposed to be their home. According to a team of researchers from the University of Exeter, most captive-born predators die if they’re released. </td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>advocate</b> 지지자
        </p>
        <p>
          <b>captivity</b> 감금
        </p>
        <p>
          <b>critical</b> 대단히 중요한
        </p>
        <p>
          <b>awareness</b> 의식
        </p>
        <p>
          <b>conservation</b> (자연 환경) 보호
        </p>
        <p>
          <b>endangered</b> 멸종 위기에 처한
        </p>
        <p>
          <b>haven</b> 안식처
        </p>
        <p>
          <b>ivory</b> 상아
        </p>
        <p>
          <b>surroundings</b> 환경
        </p>
        <p>
          <b>ostracize</b> 외면하다
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >동물원은 지구상의 서로 다른 종류의 동물들에 대해 사람들에게 교육시키는 중요한 역할을 합니다. 요즘 동물원들은 다양한 환경 문제에 대해 경각심을 높이고 보존의 중요성을 강조하기 위해 노력합니다. 동물원의 직원들은 종종 발표를 하기 위해 학교를 방문합니다. 게다가 많은 학생들은 위험에 처한 종에 대한 지식을 넓히기 위해 동물원을 방문합니다. 그들은 또한 멀리 여행을 하지 않아도 전반적으로 동물들에 대해 더 많이 배울 수 있습니다. 더욱이 동물원은 많은 동물들, 특히 그들의 털과 상아 때문에 종종 사냥을 당하는 동물들에게 안식처가 되어줍니다. </td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >그들은 꽉 막혀있는 곳에 갇혀 있기 때문에 동물원 동물들은 엄청난 스트레스를 겪습니다. 그것들을 가두는 것은 그들의 자유를 빼앗고, 동물원에서 태어난 동물들은 바깥 세상을 경험할 기회를 결코 얻지 못합니다. 그리고 그것들을 야생에 풀어주며 새로운 환경에 적응하는 것이 어렵습니다. 그것들은 그들의 집이 되어야 할 곳에서 추방당하며 자신과 같은 종류들로부터 외면당하는 경향이 있습니다. 엑시터 대학의 연구팀에 따르면 잡힌 채 태어난 대부분의 포식자들은 풀려나면 죽습니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Have you been to a zoo? What is it like?</li>
          <li>What kind of animals do people see in the zoo?</li>
          <li>Do zoos cause more harm than good in animals? Why or why not?</li>
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
