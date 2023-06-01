<script setup lang="ts">
import Contributor from "./Contributor.vue";
import IconColorLogo from "./icons/IconColorLogo.vue";
import Intro from "./Intro.vue";
import Download from "./Download.vue";
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
<main class="main">
  <div class="inner">
    <div>
      <Intro/>
    </div>
    <Download/>
    <section>
      <h3 class="tertiary-title">About</h3>
    </section>
    <section>
      <h3 class="tertiary-title">Contributors</h3>
     <Contributor
        v-for="contributor in contributors"
        :github="contributor.githubHandle"
        :linkedin="contributor.linkedin"
        :name="contributor.name"
      />
    </section>
  </div>
</main>
</template>

<style scoped lang="scss">
@import '../variables.scss';
main {
  display: flex;
  justify-content: center;
 .inner {
  width: $centerProportion;
  }
  padding: 3em 0 5em 0;
  // background: linear-gradient(141deg, rgba(228,253,225,1) 0%, rgba(255,255,255,1) 59%, rgba(244,91,105,1) 100%);
}

</style>
