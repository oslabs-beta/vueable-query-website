<script setup lang="ts">
import Footer from "./components/Footer.vue";
import Main from "./components/Main.vue";
import Header from "./components/Header.vue";
</script>

<template>

  <Header />
  <div id="top">
    <div id="bottom">
      <Main />
    </div>
  </div>
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

  #top{
    width:100%;
    background-image: url('./components/icons/header_gradient.svg');
    background-position: top; /* Center the image */
    background-repeat: no-repeat; 
    background-size:contain;
  }
  #bottom{
    width:100%;
    background-image: url('./components/icons/footer_gradient.svg');
    background-position: bottom; /* Center the image */
    background-repeat: no-repeat; 
    background-size:contain;
  }



  .secondary-title {
    font-size: 48px;
  }

  .tertiary-title {
    font-size: 36px;
  }
  
</style>
