<script setup lang="ts">
import Footer from "./components/Footer.vue";
import Main from "./components/Main.vue";
import Header from "./components/Header.vue";
</script>

<template>
  <Header />
  <Main />
  <Footer />
</template>

<style lang="scss">
 @import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@800&display=swap');
 @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@700&display=swap');
 @import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');
  html, body {
    margin: 0;
    padding: 0;
    font-family: 'Lato', sans-serif;
  }

  .title {
    font-family: 'Open Sans', sans-serif;
    font-size: 72px;
  }

  .secondary-title, .tertiary-title {
    font-family: 'Montserrat', sans-serif;
  }



  .secondary-title {
    font-size: 36px;
  }
  
</style>
