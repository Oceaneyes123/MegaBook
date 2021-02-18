<template>

  <div :style = "{fontSize: fontSize + 'px'}">

    <v-container fluid ma-0 pa-0>

      <v-layout column>

        <v-flex xs12 md12>
          <v-parallax src="https://marketplace.canva.com/KvUgA/MAD3cUKvUgA/1/s2/canva-photo-of-man-in-blue-suit-jacket%2Cstriped-shirt%2C-and-eyeglasses-talking-on-the-phone-while-sitting-at-a-table-with-his-laptop-MAD3cUKvUgA.jpg" height="900" jumbotron>     
          </v-parallax>
         </v-flex> 
      
  <h2 class = "upper-header-SD1">Lesson 1
  </h2>

  <h1 class = "lower-header-SD1">Talking on the Phone 
   </h1>
  
      <div style="padding : 15px;">

        <h3 class = "border-test2-SD1">Sample Conversation 1</h3>

        <div style="padding : 16px; padding-top : 0px;">

        <v-container grid-list-md text-xs-left>
            <v-layout row wrap>


              <v-flex xs12>
                <v-card light color="#a8dadc">
                  <v-card-text class="px-10">                  
                   
                    <table style = "border-collapse: collapse;">
    
                     <tr v-for="dialog in dialogs" :key="dialog">
                     <td class = "uppertable" >{{dialog.name}}</td>
                     <td class = "lowertable" >{{dialog.speech}}</td>
                     </tr>
    
                   </table>
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>

        </div>

      <h3 class = "border-test1-SD1">Key Expressions</h3>

      <div style="padding : 16px;">

       <p>May I please speak with…?</p>

       <p>How may I be of help?</p>

       <p>I’ll meet you at around…</p>

       <p>It’s a go.</p>

      </div>

  
         <h3 class = "border-test1-SD1">Vocabulary</h3>
     
         <div style="padding : 16px;">

           <p>schedule</p>
           <p>discuss</p>
           <p>project</p>
      
         </div>
    

      <h3 class = "border-test1-SD1">Activity</h3>

      <div style="padding : 16px;">

       <p>Lets' say that you are going to use a visual aid for your presentation. How would you explain it clearly to your audience?</p>
 
      </div>


<h3 class = "border-test2-SD1">Sample Conversation 2</h3>
      <div style="padding : 16px;">

      <v-container grid-list-md text-xs-left>
            <v-layout row wrap>


              <v-flex xs12>
                <v-card light color="#a8dadc">
                  <v-card-text class="px-10">
                  
                    <table style = "border-collapse: collapse;">
    
                     <tr v-for="seconddialog in seconddialogs" :key="seconddialog">
                     <td class = "uppertable" >{{seconddialog.name}}</td>
                     <td class = "lowertable" >{{seconddialog.speech}}</td>
                     </tr>
    
                   </table>
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>

      </div>

       
         <h3 class = "border-test1-SD1">Key Expressions</h3>
     
         <div style="padding : 16px;">

           <p>Is (name of person) there?</p>
           <p>He's not here right now</p>
           <p>....at around (time)</p>
      
         </div>
     

    <h3 class = "border-test1-SD1">Activity</h3>

      <div style="padding : 16px;">

       <p>Make your own conversation using the key expressions above. Make sure each expression is used appropriately. </p>
 
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
          name:'John Brown:',
          speech:"JB Enterprise. Good morning."
        },
        {
         name:'Mike Smith:',
         speech:"Good morning. This is Mike Smith from ADG Corporation. May I please speak with John Brown?"
        },
        {
          name:'John Brown:',
          speech:"John Brown speaking. How may be of help, Mr. Smith?"
        },
        {
          name:'Mike Smith:',
          speech:"Mr. Brown, are you free tomorrow? I was wondering if we could meet for lunch to discuss the new project?"
        },
        {
          name:'John Brown:',
          speech:"Let me check my schedule... Yes, I am free. Where do you want to meet?"
        },
        {
          name:'Mike Smith:',
          speech:"How about at World's Flavors?"
        },
        {
          name:'John Brown:',
          speech:"Yes, that would be great."
        },
        {
          name:'Mike Smith:',
          speech:"Okay then, I'll meet you at around twelve."
        },
        {
          name:'John Brown:',
          speech:" It's a go. See you there. "
        },
        ],
        seconddialogs:[
        {
          name:'A:',
          speech:"Hello."
        },
        {
         name:'B:',
         speech:"Hello. Is Mike there?"
        },
        {
          name:'A:',
          speech:"I'm sorry. He's not here right now."
        },
        {
          name:'B:',
          speech:"What time will he be back?"
        },
        {
          name:'A:',
          speech:"Around three in the afternoon. May I know who's calling?"
        },
        {
          name:'B:',
          speech:"This is John, his friend."
        },
        {
          name:'A:',
          speech:"Okay. I'll tell him you called."
        },
        {
          name:'B:',
          speech:"Thank you."
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
