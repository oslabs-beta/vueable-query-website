<script setup lang="ts">
import { computed } from 'vue';
import type { ComputedRef } from 'vue';

const props = defineProps<{
  github: string,
  linkedin: string,
  name: string
}>();

/* can optionally add `?size=${pix where <= 460}` */
const gitHubAddress: ComputedRef<string> = computed(() => `https://github.com/${props.github}`);
const getPic: ComputedRef<string> = computed(() => gitHubAddress.value + '.png');
</script>

<template>
  <div class="contributor">
    <div class="contrib-container">
        <img class="profile" :src="getPic"/>
    </div>
    <div class="contrib-container">
        {{ props.name }}
        &vert;
        <a :href="gitHubAddress">
            {{ '@' + props.github }}
        </a>
        &vert;
        <a :href="props.linkedin">
          linkedin
        </a>
    </div>
  </div>
</template>

<style scoped lang="scss">
  @import '../variables.scss';
  .contributor {
    padding: 0.5rem;
    margin: 0.5rem;
    display: flex;
    flex-direction: column;
    * {
      margin: 0.5rem;
    }
  }
  .contrib-container {
    display: flex;
    align-items: center;
    color: opacity("secondaryBlack-80");
    a {
      color: opacity("secondaryBlack-80");
    }
  }
  .profile {
    $radius: 6rem;
    width: $radius;
    height: $radius;
    border-radius: calc($radius / 2);
    box-shadow: $shadow;
    border: $border;
  }
</style>
