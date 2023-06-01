<script setup lang="ts">
import IconColorLogo from "./icons/IconColorLogo.vue";
</script>

<template>
  <div id="top-gradient">
    <div>
      <div class = 'logo'>
        <IconColorLogo />
      </div>
      <h1 class="title">
        Vueable Query
      </h1>
      <h2 class="secondary-title">
        See the metrics you've been missing!
      </h2>
    </div>
</div>
</template>

<style scoped lang="scss">
  @import '../variables.scss';
  @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&family=Montserrat&family=Open+Sans&display=swap');

  h1 {
    color: opacity("primaryBlack");
    text-align: center;
    margin: 10;
  }

  .logo{
    display: flex;
    justify-content: center;
  }

  h2 {
    color: opacity("secondaryBlack-85");
    text-align: center;

  }


</style>
