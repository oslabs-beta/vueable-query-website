<script setup lang="ts">
import IconColorLogo from "./icons/IconColorLogo.vue";
</script>

<template>
  <div id="top-gradient">
    <div>
      <div class = 'logo'>
        <IconColorLogo />
      </div>
      <h1 class="title">
        Vueable Query
      </h1>
      <h2 class="secondary-title">
        See the metrics you've been missing!
      </h2>
      <div class="button-container">
        <a class="install-button" 
        href="https://chrome.google.com/webstore/detail/vueable-query/dnhcogggodnfhnnfimapejbkkihmflaa"
        >
          Install Now
        </a>
      </div>

    </div>
</div>
</template>

<style scoped lang="scss">
  @import '../variables.scss';
  @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&family=Montserrat&family=Open+Sans&display=swap');

  h1 {
    color: opacity("primaryBlack");
    text-align: center;
    margin: 10px;
  }

  .logo, .button-container {
    display: flex;
    justify-content: center;
  }

  h2 {
    color: opacity("secondaryBlack-85");
    text-align: center;
    margin: 15px;
  }



  .install-button {
  display: inline-block;
  padding: 15px 25px;
  background-color: opacity("blue-90");;
  color: opacity("primaryWhite-100");;
  text-decoration: none;
  font-weight: bold;
  border-radius: $borderRadius;
  font-size: 20px;
  margin: 10px;
  box-shadow: $shadow;
  border: $border;
}

.install-button:hover {
  background-color: opacity("blue-100");
}

.install-button:active {
  background-color: opacity("blue-95");
}

</style>
