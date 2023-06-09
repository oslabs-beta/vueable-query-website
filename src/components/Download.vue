<script setup lang="ts">
import Codeblock from './Codeblock.vue';
</script>

<template>
  <section>
    <br>
    <br>
    <h3 class="tertiary-title">Download</h3>
    <p id="download">
      Download in just four steps!
    </p>
    <Codeblock/>
    <br>
    <br>
    <p id="load">
      Then load in chrome:
    </p>
    <div>
      <img src="./gifs/loading_Extension_Demo.gif" alt="load-extension-demo">
    </div>
  </section>

</template>

<style scoped lang="scss">
@import "../variables.scss";
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&family=Montserrat&family=Open+Sans&display=swap');

  h3 {
    line-height: 44px;
    margin-bottom: 0;
  }
  
  p {
    color: opacity("secondaryBlack-80");
    font-family: 'Lato';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 29px;
  }


  img {
    box-sizing: border-box;
    width: 100%;
    max-width: 1000px;
    background: opacity("grey-100");
    border: $border;
    box-shadow: $shadow;
    border-radius: $borderRadius;
  }
</style>