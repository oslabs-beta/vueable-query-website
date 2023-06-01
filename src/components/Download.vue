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

    <!-- <div class="codeblock">
      <div class="codeline">
      git clone https://github.com/oslabs-beta/Vueable-query.git <br/>
      </div>
      <div class="codeline">
        $cd Vueable-Query
      </div>
      <div class="codeline">
        $npm install
      </div>
      <div class="codeline">
        npm run build
      </div>
    </div> -->
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

  .codeblock {
    box-sizing: border-box;
    // width: 988px;
    // height: 133px;
    background: #000000;
    border: $border;
    box-shadow: $shadow;
    border-radius: $borderRadius;
  }

  // .codeline {
  //   color: white;
  //   width: 187px;
  //   height: 110px;
  //   font-family: 'Montserrat';
  //   font-style: normal;
  //   font-weight: 400;
  //   font-size: 18px;
  //   line-height: 22px;
  // }

  img {
    display: block;
  }
</style>