<template>

  <v-app style="
 
 background: #ED213A;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #93291E, #ED213A);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #93291E, #ED213A); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

">
  <!-- #000428,#1D4350, #004e92 --> 
  <HeaderMenu />  
      <v-main style=" position: relative; background-color: #E0E0E0; z-index: 2;margin-bottom: 305px;
  box-shadow: 10px 10px 5px #0004;">
  <!-- background-color: #7f5a83;
  background-image: linear-gradient(315deg, #7f5a83 0%, #0d324d 74%); background-color: white -->
           <Nuxt />
      </v-main>
       
       
  <FooterPage />
      
  </v-app>
</template>

<script>

import HeaderMenu from '~/components/HeaderMenu.vue'
import FooterPage from '~/components/FooterPage.vue'
export default {
 HeaderMenu,
 FooterPage}
</script>
<style>

</style> 