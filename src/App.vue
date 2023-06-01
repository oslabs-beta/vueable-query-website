<script setup lang="ts">
import Contributor from "./components/Contributor.vue";
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";

const contributors = [
  {
    githubHandle: 'annaduong94',
    linkedin: 'https://www.linkedin.com/in/anna-duong-a8719823a/'
  },
  {
    githubHandle: 'eswitbeck',
    linkedin: 'https://www.linkedin.com/in/eswitbeck/'
  },
  {
    githubHandle: 'ectjon',
    linkedin: 'https://www.linkedin.com/in/erictjon/'
  },
  {
    githubHandle: 'brand0n-y00n',
    linkedin: 'https://www.linkedin.com/in/brandon-yoon-75672a1b7/'
  },
]
</script>

<template>
  <Header />

<main>
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
    />
  </section>
</main>
<Footer />
</template>

<style lang="scss">
html, body {
  margin: 0;
  padding: 0;
}

// body {
//   background: linear-gradient(141deg, rgba(228,253,225,1) 0%, rgba(255,255,255,1) 59%, rgba(244,91,105,1) 100%);;
// }
</style>
