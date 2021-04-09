<template>
  <v-btn :to="{ name: link }" :exact="exact" :color="color" class="mx-1">
    <slot />
  </v-btn>
</template>

<script>
export default {
  props: ["exact", "link", "color"],
};
</script>
