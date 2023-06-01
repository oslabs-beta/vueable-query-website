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
    </div>
</div>
</template>

<style scoped lang="scss">
  @import '../variables.scss';
  @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&family=Montserrat&family=Open+Sans&display=swap');

  h1 {
    color: opacity("primaryBlack");
    text-align: center;
    margin: 0;
  }

  .logo{
    display: flex;
    justify-content: center;
  }

  h2 {
    color: opacity("secondaryBlack-85");
    text-align: center;
    margin: 0;
  }

  #top-gradient {
    width: 100%;
    background: radial-gradient(123.15% 389.49% at -2% 6.91%, #028090 0%, #FDF6F5 29.81%, #E4FDE1 61.77%, #FDF6F5 100%);
  }

</style>
