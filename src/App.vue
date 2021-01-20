<template>
  <v-app id="inspire"> 
    <Header></Header>
    <v-main class="white lighten-3">

      <v-container
      fluid
      class="pa-0"
      >
        <v-row>
          <v-col 
          cols="12"          
          >
           <v-img
           lazy-src="https://picsum.photos/id/11/10/6"    
           max-height="500"     
           src="./assets/container2.jpg"
           > 
          </v-img>
          </v-col>      
        </v-row>
      </v-container>
      <v-container
      fluid
      color="white"
      class="pa-0 mb-5"      
      >
        <v-row>
          <v-col
          cols="12"
          class="d-flex justify-center flex-column"
          
          >
            <v-row class="ma-0 justify-center">
              <h1>GIUSSANI DANIELE</h1>
            </v-row>
            <v-row class="ma-0 justify-center">
              <h3>Web Developer</h3>
            </v-row>

            <v-row class="d-flex ma-5 flex-row justify-center" >
              <v-btn
              class="btn ma-5 white--text"
              color="red"
              
              >
                {{ ciao }}
              </v-btn>
              <v-btn 
              class="btn ma-5 white--text"
              color="black"
              >
                {{ bye }}
              </v-btn>
            </v-row>          
            
          </v-col>   
          

        </v-row>

      </v-container>
    
    </v-main>  
    <Footer></Footer>
    
  </v-app>
</template>

<script>

import Header from './components/Header.vue'
import Footer from './components/Footer.vue'


  export default {

      data: () => ({      
      ciao: 'ESPLORA',
      bye: 'Hello',
    }),
      components: {
      Header, 
      Footer,           
    }  
    
  }
</script>

<style scoped>
  h1 {
    font-size: 70px;
    font-family:'Courier New', Courier, monospace;
  }
  h3 {
    font-size: 40px;
    font-family:'Courier New', Courier, monospace;
  
  }
  .btn {
    font-family: 'Courier New', Courier, monospace;
  }
</style>