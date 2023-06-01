<script setup lang="ts">
import IconColorLogo from "./icons/IconColorLogo.vue";
</script>

<template>
  <div>
    <div class = 'logo'>
      <IconColorLogo />
    </div>
    <h1>
      Vueable Query
    </h1>
    <h2>
      See the metrics you've been missing!
    </h2>
  </div>
</template>

<style scoped lang="scss">
  @import '../variables.scss';
  @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&family=Montserrat&family=Open+Sans&display=swap');

  h1 {

    font-size: 72px;
    font-family: "Open Sans";
    color: opacity("primaryBlack");
    text-align: center;
    font-weight: 800;
  }
  .logo{
    display: flex;
    justify-content: center;
  }

  h2 {
    font-size: 48px;
    font-family: "Montserrat";
    color: opacity("secondaryBlack-85");
    text-align: center;
    font-weight: 700;
  }
</style>