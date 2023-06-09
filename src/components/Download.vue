<script setup lang="ts">
import Codeblock from './Codeblock.vue';
</script>

<template>
  <section>
    <h3 class="tertiary-title">Alternate Download</h3>
    <p id="download">
      Want to download the source code and build your own extension?<br>
      Download from GitHub and build the extension with the following commands.<br>
      Then load the dist folder in Google Chrome as an unpacked Chrome Extension.
    </p>
    <Codeblock/>
    <br>
    <!-- <div>
      <img src="./gifs/loading_Extension_Demo.gif" alt="load-extension-demo">
    </div> -->
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