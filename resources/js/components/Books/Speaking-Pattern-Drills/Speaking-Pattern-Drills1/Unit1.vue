<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>

       
         <v-flex xs12 md12>
          <v-parallax src="https://marketplace.canva.com/aW8V0/MAD0iWaW8V0/1/s2/canva-conversation-between-job-applicant-and-representative-employer-MAD0iWaW8V0.jpg">
           
          </v-parallax>
         </v-flex>
        
        
  <h3 class = "upper-header-SPD1">PATTERN 1
  </h3>
  
  
 
        <h1 class = "lower-header-SPD1">I think
        </h1>
 
      <div style="padding : 15px;">
        <div style="padding : 16px; padding-top : 0px;">

        <p>I think the movie's almost over.</p>

        <p>I think I saw him before.</p>

        <p>I think it is going to rain soon.</p>
        
        <p>I think we should get going.</p>

        </div>

      <h3 class = "border-SPD1 white--text">EXERCISE 1</h3>

      <div style="padding : 16px;">

        <p>Fill in the blanks with I don't think.</p>

        <table style = "border-collapse: collapse;">
    
          <tr v-for="dialog in dialogs" :key="dialog">
            <td class = "uppertable" >{{dialog.name}}</td>
            <td class = "lowertable" >{{dialog.speech}}</td>
          </tr>
    
        </table>

      </div>

      <h3 class = "border-SPD1 white--text">VOCABULARY</h3>

      <div style="padding : 16px;">

      <p>
        <b>Movie</b> – A form of entertainment that enacts a story by
                       sound and a sequence of images giving the illusion of
                       continuous movement
      </p>

      <p>Example: I think we should watch this movie instead.</p>

      <p><b>Over</b> – Having come or been brought to a conclusion; done</p>

      <p>Example: I think the storm is over.</p>

      </div>

      <h3 class = "border-SPD1 white--text">Expressions</h3>

      <div style="padding : 16px;">

      <p>
        <b>Get going</b> – Get moving
      </p>

      <p>Example: I think I better get going, it’s getting late</p>

      <p><b>No choice</b> – No other options</p>

      <p>Example: I think I have no choice but to talk to you.</p>

      </div>

      <h3 class = "border-SPD1 white--text">EXERCISE 2</h3>

      <div style="padding : 16px;">

        <p>Fill in the blanks with the vocabulary or expressions
           found on top.
        </p>

        <ol style="margin: 12px;">

          <li>Let’s ______________ or we will be late for school.
          </li>

          <li>The party is __________ let’s all go home.
          </li>

          <li>I have ______________ but to join you or I will be left all alone here.
          </li>

          <li>The ___________ really moved me to tears.
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

  props: ['fontSize'],

  data(){

    return{
        dialogs:[
        {
          name:'A:',
          speech:"______________ we should get going."
        },
        {
         name:'B:',
         speech:"Already? But it's not even 5 yet."
        },
        {
          name:'A:',
          speech:"I know, but ______________ it's going to rain soon."
        },
        {
          name:'B:',
          speech:'I guess we have no choice then.'
        },
        ],
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

<style scoped lang="css">

p{

  margin-top: 10px;
}

body{

  font-size: 16px;
}


</style>
