<script setup lang="ts">
import { ref } from "vue";
import IconGithub from "./icons/IconGithub.vue";
import IconLinkedin from "./icons/IconLinkedin.vue";
import IconLogo from "./icons/IconLogo.vue";
import IconMedium from "./icons/IconMedium.vue";
</script>

<template>
  <div id="header-container">
    <header>
      <div class="title-group">
        <h3>
          <IconLogo/> Vueable Query
        </h3>
      </div>
      <div class="links-group">
        <a href="https://github.com/oslabs-beta/Vueable-query">
          <IconGithub/>
        </a>
        <span>|</span>
        <a href="https://www.linkedin.com/company/vueable-query/?viewAsMember=true">
          <IconLinkedin/>
        </a>
        <span>|</span>
        <a href="">
          <IconMedium/>
        </a>
      </div>
    </header>
  </div>
</template>

<style scoped lang="scss">
@import "../variables.scss";
  
  #header-container {
    display: flex;
    background-color: opacity("pink-100");
    justify-content: center;
    border-bottom: $border;
    box-shadow: $shadow;
  }
  .links-group, .title-group, .title-group h3 {
    display: flex;
    align-items: center;
    column-gap: 5px;
  }
  header{
    width: $centerProportion;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }  
  span {
    font-size: 30px;
  }
  h3 {
    font-family: "Open Sans";
    font-size: 24px;
    margin: 15px;
    text-align: center;
  }
  a{
    margin-left: 10px;
    margin-right: 10px;
    color: black;
  }
</style>
