<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://images.pexels.com/photos/2342585/pexels-photo-2342585.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should We Ban Rap Music In Schools?
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
      <td class = "lowertable" >Rap is bad news. Lyrics often preach to children advocating a criminal lifestyle. Many rappers write threatening ‘diss’ tracks that push for violence against other rappers. When Tupac Shakur wrote the song, “Hit Em Up” he insulted Notorious B.I.G., and aggressively yelled obscenities, threats, and insults. In doing so, many argue that it only increased the rivalry between both rappers, causing their fans to kill both rappers with guns. One can argue that such aggressive content in their lyrics only worsened the violence. If we allow our children to listen to such music they will only explore a deep culture of violence.</td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Victoria :</b></td>
      <td class = "lowertable" >Rap is simply music. Today’s rap is not music that is anything violent, but music which advocates living well, maybe carelessly. In keeping with this, rap music is harmless in nature. When we consider the many crimes of rappers in America and Korea, most only involve their possession of something illegal and no actual violent crime. Despite the fact that such acts may be shameful, they did not harm anyone or inspire children to harm others. In fact, many rappers have charitable hearts. People like Jay-Z, Eminem, and P.Diddy donate money to help those in need.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>lyric</b> 가사
        </p>
        <p>
          <b>preach</b> 설교하다, 전하다
        </p>
        <p>
          <b>advocate</b> 지지하다, 옹호하다
        </p>
        <p>
          <b>threatening</b> 위협하는
        </p>
        <p>
          <b>obscenity</b> 외설
        </p>
        <p>
          <b>threat</b> 위협
        </p>
        <p>
          <b>insult</b> 모욕
        </p>
  </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>David :</b></td>
            <td class = "lowertable" >랩은 나쁜 소식입니다. 가사는 자주 아이들이 범죄적인 생활습관을 지지하도록 전합니다. 많은 래퍼들이 다른 래퍼들을 향해 폭력을 요구하는 위협적인 ‘디스’ 곡들을 만듭니다. 투팍 샤커는 “Hit Em Up”이라는 노래를 작곡하였을 때 그는 노토리어스 비아이지를 모욕하였고 공격적으로 외설행위, 위협 그리고 모욕을 노래했습니다. 그렇게 함으로써, 많은 이들은 이것이 두 래퍼 사이의 라이벌 관계를 증가시켰으며, 이것은 그들의 팬들이 총으로 두 래퍼를 쏴 죽이게 했다고 주장합니다. 누군가는 그들의 가사에 이러한 공격적인 내용이 담겨 있는 것은 폭력을 악화시킬 뿐이라고 주장합니다. 만약 우리의 아이들이 이러한 음악을 듣도록 허용한다면, 그들은 폭력의 깊은 문화만을 탐구하게 될 것입니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Victoria :</b></td>
            <td class = "lowertable" >랩은 간단하게 말해서 음악일 뿐입니다. 오늘날의 랩은 폭력적인 음악이 아니라, 잘 지내는 태평한 삶을 옹호하는 음악입니다. 이와 함께, 랩 음악은 본질상 무해합니다. 우리가 미국과 한국의 래퍼들의 많은 범죄들을 고려해 보면, 대부분은 불법적인 무엇인가에 대한 소유를 수반할 뿐이며 실제로 폭력적인 범죄는 없습니다. 이러한 행동이 수치스러울지도 모른다는 사실에도 불구하고, 이것들은 누구에게도 해를 가하지 않고 아이들이 다른 사람에 해를 가하도록 부추기지도 않습니다. 사실상, 많은 래퍼들이 자선적인 마음을 갖고 있습니다. 제이 지, 에미넴 그리고 P.Diddy와 같은 사람들은 곤경에 처한 사람들을 돕기 위해 돈을 기부합니다.</td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>Do you listen to rap music? If yes, who is your favorite rapper? If not, what kind of music do you usually listen to?</li>
          <li>What do you think of the message that rap music brings to its listeners?</li>
          <li>How does rap music affect the youth?</li>
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
