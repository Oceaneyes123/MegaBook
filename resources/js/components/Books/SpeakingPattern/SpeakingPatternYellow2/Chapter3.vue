<template>

<div :style = "{fontSize: fontSize + 'px'}">

<v-container fluid ma-0 pa-0>

  <v-layout column>
    <v-img
           src="https://image.freepik.com/free-photo/automobile-accident-street_158538-10306.jpg">

        <v-layout
        align-end
        fill-height
        pa-2
        black--text
      >
     <h1 class="upper-header-SPY2">~가 있었어
  </h1>
      </v-layout>
    </v-img>


          <h2 class="lower-header-SPY2">Today's topic</h2>

  <hr width="60%">
               <div style="padding : 10px; line-height: 200%;">

                 <h2>Pattern 23 |  </h2>
                  <br />
                  <h3>There has been…</h3>
                    <br />
                    <p>
                    There was…(~가 있었다) 가 과거에 일어나서 이미 끝난 일을 말할 때 쓰는 표현이라면, there has been… 은 과거부터 지금까지 계속 있어온 일을 말할 때, 또는 과거에 있었던 일이 지금까지 영향을 미칠 때 사용한다.
                    </p>
                    <br />

<h2 class = "border-SPY2">Dialogue
</h2>

<div style="padding-top : 10px; padding-bottom : 2px;">

          <br />
          <p style="line-height: 2;">
            A : I have some bad news.<br />
            B : What is it?<br />
            A : <b>To where?</b><br />
            B : Is anyone hurt?
          </p>
          <p style="line-height: 2;">
            A : 안 좋은 소식이야.<br />
            B : 뭔데?<br />
            A : <mark style="background-color: #a7d7c5; color: #d9e7cd;">There has been an accident.</mark><br />
            B : 누가 다쳤어?
          </p>
          <br />


</div>

<h2  class = "border-SPY2">Pattern Practice
</h2>

<div style="padding-top : 10px; padding-bottom : 0px;">

        <br />

        <p>
          &rarr; 우리말을 보고 순식간에 영어로 말할 수 있을 때까지 반복하세요!
        </p>
        <br />

        <p>
          <b>177</b> 사고가 났어. ( accident ) <br />
        </p>
        <p>
          <b>178</b> 바뀐 게 좀 있어. ( change ) <br />
        </p>
        <p>
          <b>179</b> 준비할 시간이 별로 없었어. ( prepare ) <br />
        </p>
        <p>
          <b>180</b> 오해가 있었어요. ( misunderstanding ) <br />
        </p>
        <p>
          <b>181</b> 계획에 변경이 생겼어 ( change, plan ) <br />
        </p>
        <p>
          <b>182</b> 그들 사이에 갈등이 있었습니다. ( conflict, between )<br />
        </p>
        <p>
          <b>183</b> 발전이 있었습니다. ( improvement )<br />
        </p>
        <p>
          <b>184</b> 착오가 있었습니다. ( mistake ) <br />
        </p>

        <v-container grid-list-md text-xs-left>
      <v-layout row wrap>


          <v-flex xs12>
          <v-card light color="#a7d7c5">
            <v-card-text class="px-10" style="color:#d9e7cd;">
              177 There has been an accident.<br />
              178 There has been some changes.<br />
              179 There has been little time to prepare.<br />
              180 There has been a misunderstanding. <br />
              181 There has been a change in the plan.<br />
              182 There has been a conflict between them.<br />
              183 There has been an improvement.<br />
              184 There has been a  mistake.<br />
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
  </v-container>
        
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


    }

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

<style lang="css">

p{

  margin-top: 10px;
}

h3{
  padding-top: 7px;

}


body{

  font-size: 16px;
}

</style>
