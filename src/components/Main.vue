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

  <div class="spacing">
    <div class="inner">
      <div>
        <Intro/>
      </div>
      <div id="mid-gradient">
        <Download/>
        <h3 class="tertiary-title">Features</h3>
          <ul>
            <li>A timeline to visualize the query history</li>
            <li>A text panel to display all relevant queries under their query key</li>
            <li>Highlighting on click and hover</li>
            <li>Tooltip displayed on hover</li>
          </ul>
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
  li{  
    color: opacity("secondaryBlack-80");
    font-family: 'Lato';
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
  }
 .inner {
  width: $centerProportion;
  }
  padding: 3em 0 5em 0;
  /*background-color: opacity("secondaryWhite");*/
}
</style>
