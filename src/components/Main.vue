<script setup lang="ts">
import Contributor from "./Contributor.vue";
import Intro from "./Intro.vue";
import Download from "./Download.vue";
import Demo from "./Demo.vue";
const contributors = [
  {
    githubHandle: 'annaduong94',
    linkedin: 'https://www.linkedin.com/in/anna-duong-a8719823a/',
    name: 'Anna Duong'
  },
  {
    githubHandle: 'eswitbeck',
    linkedin: 'https://www.linkedin.com/in/esther-witbeck/',
    name: 'Esther Witbeck'
  },
  {
    githubHandle: 'ectjon',
    linkedin: 'https://www.linkedin.com/in/erictjon/',
    name: 'Eric Tjon'
  },
  {
    githubHandle: 'brand0n-y00n',
    linkedin: 'https://www.linkedin.com/in/brandon-yoon-75672a1b7/',
    name: 'Brandon Yoon'
  },
]
</script>

<template>
  <main>
  <!-- <HeaderGradient/> -->
  <div class="spacing">
    <div class="inner">
      <div>
        <Intro/>
      </div>
      <div id="mid-gradient">
        <Download/>
        <section>
          <h3 class="tertiary-title">About</h3>
        </section>
        <Demo />
        <section id="bottom-gradient">
        <h3 class="tertiary-title">Contributors</h3>
        <div>
          <Contributor 
            v-for="contributor in contributors"
            :github="contributor.githubHandle"
            :linkedin="contributor.linkedin"
            :name="contributor.name"
          />
        </div>
        </section>
    </div>
  </div>
  </div>
  <!-- <FooterGradient/> -->
</main>
</template>

<style scoped lang="scss">
@import '../variables.scss';
main {
  display: flex;
  justify-content: center;
  .spacing {
    width: 100%;
    display: flex;
    justify-content: center;
  }
 .inner {
  width: $centerProportion;
  }
  padding: 3em 0 5em 0;
  /*background-color: opacity("secondaryWhite");*/
}
</style>
