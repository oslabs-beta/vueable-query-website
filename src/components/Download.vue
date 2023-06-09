<script setup lang="ts">
import Codeblock from './Codeblock.vue';
</script>

<template>
  <section>
    <br>
    <br>
    <h3 class="tertiary-title">Download</h3>
    <div>
      <p> Check us out on the Chrome Extension store! </p>
      <a class="install-button" href="https://chrome.google.com/webstore/detail/vueable-query/dnhcogggodnfhnnfimapejbkkihmflaa">Install Now</a>
    </div>
    <p id="download">
      Or download from GitHub in 4 steps
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

  .install-button {
  display: inline-block;
  padding: 10px 20px;
  background-color: #4CAF50;
  color: #FFFFFF;
  text-decoration: none;
  font-weight: bold;
  border-radius: 4px;
}

.install-button:hover {
  background-color: #45a049;
}

.install-button:active {
  background-color: #3e8e41;
}
</style>