<script setup lang="ts">
</script>

<template>
  <footer>
    <div class="inner">
      <div class="col">
        <a
        href="https://github.com/oslabs-beta/Vueable-query/blob/main/LICENSE">Licensed with the MIT license</a>
      </div>
      <div class="col">
        <a href="https://github.com/oslabs-beta/Vueable-query/blob/main/CONTRIBUTING.md">Interested in contributing?</a>
      </div>
      <div class="col">
        <a href="https://github.com/oslabs-beta/Vueable-query/">GitHub Repo</a>
        <a href="">Medium Article</a>
        <a href="https://www.linkedin.com/company/vueable-query/about/">LinkedIn</a>
        <a href="">Hacker News Post</a>
      </div>
    </div>
  </footer>
</template>

<style scoped lang="scss">
  @import '../variables.scss';
  footer {
    padding: 2rem;
    background: opacity("grey-100");
    border-top: $border;
    display: flex;
    justify-content: center;
    margin-top: 3rem;

    .inner {
      width: 75%;
      display: flex;
      justify-content: space-between;

      > * {
        padding: 1rem;
      }
    }
    
    a {
      color: opacity("secondaryBlack-80");
    }
  }

  .col {
    display: flex;
    flex-direction: column;
    * {
      margin: .1rem;
    }
  }
  
</style>
