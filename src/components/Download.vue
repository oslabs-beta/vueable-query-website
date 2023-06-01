<script setup lang="ts">
import Codeblock from './Codeblock.vue';
</script>

<template>
  <section>
    
    <h3>Download</h3>
    <p id="download">
      Download in just four steps!
    </p>
    
    <Codeblock/>


    <p id="load">
      Then load in chrome:
      <div>
        <img src="./gifs/loading_Extension_Demo.gif" alt="load-extension-demo">
      </div>
    </p>
  </section>

</template>

<style scoped lang="scss">
@import "../variables.scss";
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&family=Montserrat&family=Open+Sans&display=swap');

  h3 {
    // position: absolute;
    // width: 388px;
    // height: 45px;
    color: opacity("primaryBlack-85");
    font-size: 36px;
    font-family: "Montserrat";
    font-weight: 700;
    line-height: 44px;
    margin-bottom: 0;
  }
  
  p {
    color: opacity("secondaryBlack-80");
    // position: absolute;
    // width: 388px;

    font-family: 'Lato';
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
  }

  #download {
    height: 58px;
    margin-bottom: 0;
  }

  #load {
    height: 29px;
  }


  img {
    box-sizing: border-box;
    width: 428px;
 
    background: #E7E7E7;
    border: 1px solid rgba(7, 29, 36, 0.3);
    box-shadow: 0px 8px 8px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
  }
</style>