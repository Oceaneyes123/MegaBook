<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>
        <v-img src="https://image.freepik.com/free-photo/front-view-man-putting-his-referendum-ballot-box_23-2148265556.jpg" style="max-width: 100%; display:block; height: auto;">

        <v-layout
        align-end
        fill-height
        pa-0
        white--text
        >

        <transition name="slide-fade">
        <h1 v-if="showTitle" class = "upper-header-lg">Should Felons Be Allowed to Vote?
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
      <td class = "uppertable" ><b>Henry :</b></td>
      <td class = "lowertable" >Felons should be allowed to vote. After completing their sentence, they are free to get married, own property, drive, and buy alcohol, so why should they be banned from voting? Steve Chapman, a columnist at the Chicago Tribune, said, “In many places, the assumption is that they can’t be trusted to help choose our leaders. If we thought criminals could never be reformed, we wouldn’t let them out of prison in the first place.” Plus, disfranchisement is unconstitutional. The Eighth Amendment prohibits excessive sanctions. </td>
    </tr>
    <tr class = "second-dialog-lg">
      <td class = "uppertable" ><b>Ashley :</b></td>
      <td class = "lowertable" >Some states already allow felons to vote. Vermont and Maine, for instance, grant felons the right to vote while in prison, while 10 other states have strict restrictions. It should be up to the state whether or not a felon gets to vote in elections. Allowing felons to vote is a state prerogative, not a federal one. According to The Washington Times, “Congress should let the process play itself out, as the Constitution allows it to.” Also, the right to vote should not be restored automatically.</td>
    </tr>

    </table>

      <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Vocabulary</h3>

      <div style="padding : 16px;">

        <p>
          <b>felony</b> 중죄
        </p>
        <p>
          <b>bar</b> ~에게 (~하는 것을) 금(지)하다
        </p>
        <p>
          <b>disenfranchisement</b> 선거권 박탈
        </p>
        <p>
          <b>deprive</b> 빼앗다
        </p>
        <p>
          <b>unconstitutional</b> 헌법에 위배되는
        </p>
        <p>
          <b>excessive</b> 지나친, 과도한
        </p>
        <p>
          <b>sanction</b> 처벌, 벌칙
        </p>
        <p>
          <b>prerogative</b> 특권
        </p>
        <p>
          <b>federal</b> 연방 정부의
        </p>

      </div>

      <div class ="line-lg">
      </div>
      <h3 class = "border-translate-lg white--text">해석</h3>

      <div style="padding : 16px;">

        <table class = "standard-table">

          <tr>
            <td class = "uppertable" ><b>Henry :</b></td>
            <td class = "lowertable" >중죄인은 투표 할 수 있어야 합니다. 형기를 마친 이들은 자유롭게 결혼하고, 재산도 소유하고, 운전도 하고, 술도 사는데, 왜 투표를 금지해야 할까요? 시카고 트리뷴 칼럼니스트 인 스티브 채프먼은 “많은 곳에서 그들은 우리들의 지도자 선택에 있어서 도움을 준다고 신뢰받을 수 없다고 가정합니다. 범죄자들을 개혁 할 수 없다고 생각했다면, 우선 감옥에서 내보내지는 않았을 것입니다.” 게다가, 박탈은 위헌입니다. 제 8조 수정 조한은 과도한 제재를 금지하고 있습니다.</td>
          </tr>
          <tr class = "second-dialog-lg">
            <td class = "uppertable" ><b>Ashley :</b></td>
            <td class = "lowertable" >일부 주에서는 이미 중죄인의 투표를 허용하고 있습니다. 예를 들어, 버몬트와 메인주는 중죄인에게 감옥에 있는 동안 투표권을 부여하고, 다른 10개 주는 엄격한 규제를 가합니다. 중죄인은 선거에서 투표 할 수 있는지 여부는 그것은 주정부에 달려있어야 합니다. 중죄인에게 투표하도록 허용하는 것은 주 특권이 있는 것이지, 연방 특권이 있는 것은 아닙니다. 워싱턴 타임스에 따르면, "의회는 헌법이 허용하는 대로 그 절차 자체를 진행하도록 해야 한다"라고 합니다." 또 투표권이 자동으로 복구돼서는 안 됩니다. </td>
          </tr>

          </table>


      </div>

    <div class = "line-lg">
      </div>
      <h3 class = "border-lg white--text">Questions</h3>

      <div style="padding : 16px;">

        <ol style="margin: 12px;">
          <li>What are the most common felonies in your country?</li>
          <li>Are felons allowed to vote in your country? Should they be allowed? Why or why not?</li>
          <li>Why is voting important?</li>
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
