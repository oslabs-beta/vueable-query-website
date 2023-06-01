<script setup lang="ts">
import Footer from "./components/Footer.vue";
import Main from "./components/Main.vue";
import Header from "./components/Header.vue";
</script>

<template>
<<<<<<< HEAD
  <Header />

<main id="main">
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
=======
<Header />
<Main />
>>>>>>> 61b4e69ad4f6fe83e6728328c833aea4a5e7276c
<Footer />
</template>

<style lang="scss">
html, body {
  margin: 0;
  padding: 0;
  
}
#main {
  background: linear-gradient(141deg, rgba(228,253,225,1) 0%, rgba(255,255,255,1) 59%, rgba(244,91,105,1) 100%);
}
// body {
//   background: linear-gradient(141deg, rgba(228,253,225,1) 0%, rgba(255,255,255,1) 59%, rgba(244,91,105,1) 100%);;
// }
</style>
