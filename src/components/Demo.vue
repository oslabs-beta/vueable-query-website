<script setup lang="ts">
</script>

<template>
  <h3 class="tertiary-title">
    Demo
  </h3>
  <div>
    <img src="./gifs/demo.gif" alt="devtools-demo">
  </div>
</template>

<style scoped lang="scss">
  @import "../variables.scss";

  img {
    box-sizing: border-box;
    width: 100%;
    background: opacity("grey-100");
    border: $border;
    box-shadow: $shadow;
    border-radius: $borderRadius;
  }
</style>