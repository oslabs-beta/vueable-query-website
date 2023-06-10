<script setup lang="ts">
  import Codeline from "./Codeline.vue";
</script>

<template>
  <div class="codeblock">
    <Codeline
      :text="'git clone https://github.com/oslabs-beta/Vueable-query.git'"
    />
    <Codeline
      :text="'cd Vueable-Query'"
    />
    <Codeline
      :text="'npm install'"
    />
    <Codeline
      :text="'npm run build'"
    />
  </div>
</template>

<style lang="scss">
  @import "../variables.scss";
  @import url('https://fonts.googleapis.com/css2?family=Ubuntu+Mono&display=swap');
  .codeblock {
    padding: 1rem;
    border-radius: $borderRadius;
    background-color: opacity("secondaryBlack-100");
    color: opacity("primaryWhite-100");;
    font-family: 'Ubuntu Mono', monospace;
    border: $border;
    box-shadow: $shadow;
    }
</style>
