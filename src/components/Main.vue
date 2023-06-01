<script setup lang="ts">
import Contributor from "./Contributor.vue";
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
  <div class="inner">
    <div>
      <svg>
      </svg>
      <h1>
        Vueable Query
      </h1>
      <h2>
        See the metrics you've been missing
      </h2>
    </div>
    <section>
      <h3>Download</h3>
      <p>
        Download in just four steps
      </p>
      <div class="codeblock">
        <div class="codeline">
        git clone https://github.com/oslabs-beta/Vueable-query.git <br/>
        </div>
        <div class="codeline">
          cd Vueable-Query
        </div>
        <div class="codeline">
          npm install
        </div>
        <div class="codeline">
          npm run build
        </div>
      </div>
      <p>
        Then load in chrome:
      </p>
    </section>
    <section>
      <h3>About</h3>
    </section>
    <section>
      <h3>Contributors</h3>
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
}

</style>
