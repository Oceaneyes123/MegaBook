<template>
  <div :style="{ fontSize: fontSize + 'px' }">
    <v-container fluid ma-0 pa-0>
      <v-layout column>
        <v-img
          src="https://image.freepik.com/free-photo/happy-successful-businessman_53876-89038.jpg"
          style="max-width: 100%; display: block; height: auto"
        >
          <v-layout align-end fill-height pa-0 white--text>
            <transition name="slide-fade">
              <h1 v-if="showTitle" class="upper-header-lg">
                Happiness Is More Important Than Success
              </h1>
            </transition>
          </v-layout>
        </v-img>

        <div class="line-top-lg"></div>
        <h3 class="lower-header-lg white--text">Topic</h3>

        <div style="padding: 16px; line-height: 1.6">
          <table class="standard-table">
            <tr>
              <td class="uppertable"><b>David :</b></td>
              <td class="lowertable">
                Plenty of graduates of Ivy League universities end up not
                working for large corporations or prestigious organizations.
                Rather, they do what they want instead of what society thinks
                they should do. Many people pursue financially rewarding careers
                like law, business, medicine, and finance, which often means
                long hours (especially in Korea), stressful work, and demanding
                bosses. Despite their high salaries, many are unhappy doing
                something they never really wanted to do, and the trend is to
                seek greater meaning in both occupation and life. So happiness
                does trump success.
              </td>
            </tr>
            <tr class="second-dialog-lg">
              <td class="uppertable"><b>Victoria :</b></td>
              <td class="lowertable">
                While being happy is important, success can make life easier and
                thus happier. So many self-help books and gurus tell people to
                do what they love, but a large number of professions promise low
                pay and stressful work like teaching and art. What good is life
                if doing something one wants means always struggling to pay the
                bills and worrying about money? For many, having a happy life
                means earning enough to afford family necessities like a nice
                home or things for the children. So success often brings about
                happiness. In other words, one can have both.
              </td>
            </tr>
          </table>

          <div class="line-lg"></div>
          <h3 class="border-lg white--text">Vocabulary</h3>

          <div style="padding: 16px">
            <p><b>security</b> 보장</p>
            <p><b>prestigious</b> 일류의</p>
            <p><b>trump</b> 으뜸패를 내다</p>
            <p><b>trend</b> 동향</p>
            <p><b>guru</b> 구루</p>
          </div>

          <div class="line-lg"></div>
          <h3 class="border-translate-lg white--text">해석</h3>

          <div style="padding: 16px">
            <table class="standard-table">
              <tr>
                <td class="uppertable"><b>David :</b></td>
                <td class="lowertable">
                  아이비리그 대학의 많은 졸업자들은 대기업이나 명망 있는
                  조직에서 일하지 않게 됩니다. 오히려, 그들은 사회가 그들이 해야
                  한다고 생각하는 것을 하는 대신 그들이 원하는 것을 합니다. 많은
                  사람들이 자주 (특히 한국은) 긴 업무 시간과 스트레스가 많은
                  직업 그리고 까다로운 상사를의미하는 법, 기업, 의학 그리고
                  재무와 같은 재정적으로 보상이 좋은 커리어를 추구합니다. 높은
                  봉급에도 불구하고, 많은 이들은 그들이 정말 원치 않는 일을
                  하면서 불행하고, 직업과 삶 모두에서 더 큰 의미를 찾게 됩니다.
                  따라서 행복이 성공을 능가합니다.
                </td>
              </tr>
              <tr class="second-dialog-lg">
                <td class="uppertable"><b>Victoria :</b></td>
                <td class="lowertable">
                  행복한 것이 중요하지만, 성공은 삶을 더 쉽고 따라서 더 행복하게
                  만들어줄 수 있습니다. 수많은 자기계발서들과 전문가들은
                  사람들그들이 사랑하는 일을 하라고 말하지만, 많은 직업들은
                  교육과 예술 같이 낮은 봉급과 스트레스가 쌓이는 직업만을
                  약속합니다. 만약 자신이 원하는 것을 하는 것이 항상 고지서를
                  지불하고 돈에 대해 걱정하는 것을 의미한다면 무엇이 좋다는
                  것일까요? 많은 사람들에게 행복한 삶은 좋은 집과 아이들을 위한
                  물건들처럼 가족에게 필요한 것들을 제공할 만큼 충분히 돈을 버는
                  것을 의미합니다. 따라서 성공은 자주 행복을 가져옵니다. 다시
                  말해서, 우리는 둘 다 가질 수 있습니다.
                </td>
              </tr>
            </table>
          </div>

          <div class="line-lg"></div>
          <h3 class="border-lg white--text">Questions</h3>

          <div style="padding: 16px">
            <ol style="margin: 12px">
              <li>How do you define success?</li>
              <li>Are all successful people happy? Why or why not?</li>
              <li>
                Which do you think is more important? Happiness or success? Why?
              </li>
            </ol>
          </div>
        </div>
      </v-layout>
    </v-container>
  </div>
</template>



<script>
export default {
  props: ["fontSize"],

  data() {
    return {
      showTitle: false,
    };
  },

  mounted() {
    this.showTitle = true;
  },

  beforeMount() {},

  methods: {},

  watch: {
    fontSize(current, old) {
      console.log(current, "current");
      console.log(old, "previous");
    },
  },
};
</script>

<style scoped lang="css">
</style>
