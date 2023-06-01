<script setup lang="ts">
import { ref } from "vue";
import IconGithub from "./icons/IconGithub.vue";
import IconLinkedin from "./icons/IconLinkedin.vue";
import IconLogo from "./icons/IconLogo.vue";
import IconMedium from "./icons/IconMedium.vue";
</script>

<template>
  <header>
    <div class="title group">
      <a>
        <IconLogo/>
      </a>
      <h3>
        Vueable Query
      </h3>
    </div>
    <div class="links group">
      <a>
        <IconGithub/>
      </a>
      <a>
        <IconLinkedin/>
      </a>
      <a>
        <IconMedium/>
      </a>
    </div>
  </header>
</template>

<style scoped lang="scss">
@import "../variables.scss";
  .group {
    display: flex;
  }

  header {
    display: flex;
    justify-content: space-around;
    background-color: rgb(244,91,105);
  }

  h3 {
    font-family: "Open Sans";
  }
</style>