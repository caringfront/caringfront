<template>
  <div>
    <navbar />
    <div id='show_bg_2'>
        <v-row> 
          <v-spacer />
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12">
            <p class="text-center">
            <v-btn text x-large light class="text-capitalize white green--text mr-2" height="10vh">Try the app</v-btn>
            <v-btn text x-large dark class="text-capitalize green" height="10vh">Explore mobile, IoT, AI and platform solutions</v-btn>
            </p>
          </v-col>
          <v-spacer />
        </v-row>
    </div>
     <v-row>
        <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12">
          <h1 class="text-center ma-8">Our Apps</h1>
        </v-col>
        </v-row>
        <v-row class="ma-10">
        <v-col cols="12" xs="3" sm="3" md="3" lg="3" xl="3">
          <router-link to="#" custom v-slot="{ navigate }">
          <v-card class="pa-3" height="28vh" @click="navigate" role="link">
            <p class="text-center"><img class=" ma-5 mt-14" :src="require('../assets/deliveryaide_logo.png')" height="80vh"/></p>
          </v-card>
          </router-link>
          <h1 class="text-center text-h6 mt-5">Courier and delivery</h1>
        </v-col>
        <v-col cols="12" xs="3" sm="3" md="3" lg="3" xl="3">
           <router-link to="#" custom v-slot="{ navigate }">
         <v-card class="pa-3" height="28vh" @click="navigate" role="link">
            <p class="text-center"><img class="ma-5 mt-14" :src="require('../assets/medrm_logo.png')" height="80vh"/></p>
          </v-card>
           </router-link>
          <h1 class="text-center text-h6 mt-5">Healthcare and medical first responders</h1>
        </v-col>
        <v-col cols="12" xs="3" sm="3" md="3" lg="3" xl="3">
          <a target="_blank" href="https://utilitygator.mybluemix.net/">
          <v-card class="pa-3" height="28vh">
             <p class="text-center"><img class=" ma-5 mt-14" :src="require('../assets/utilitygator_logo.png')" height="80vh"/></p>
          </v-card>
          </a>
          <h1 class="text-center text-h6 mt-5">Utilities</h1>
        </v-col>
        <v-col cols="12" xs="3 text-h6" sm="3" md="3" lg="3" xl="3">
           <router-link to="#" custom v-slot="{ navigate }">
          <v-card class="pa-3" height="28vh"  @click="navigate">
            <p class="text-center"><img class=" ma-5 mt-14" :src="require('../assets/kersto_logo.png')" height="80vh"/></p>
          </v-card>
           </router-link>
          <h1 class="text-center text-h6 mt-5">Retail and e-Commerce</h1>
        </v-col>
        </v-row>
  </div>
</template>

<script>
import Navbar from '../components/Navbar.vue'
  export default {
    name: 'Home',

    components: {
        Navbar
     
    },
  }
</script>

<style>
#show_bg_2 {
    background-image:
    linear-gradient(to left, rgba(101, 233, 101, 0.247), rgba(11, 46, 4, 0.73)),
    url('../assets/showcase.jpeg');
    height: 80vh;
    background-size: cover;
    color: white;
    padding: 80px;
    padding-top: 450px;
    
}
</style>
