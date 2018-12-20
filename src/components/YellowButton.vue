<template>
  <gx-button class="yellow" :propagate="true">
    <slot></slot>
  </gx-button>
</template>
<script>
import GxButton from "./GxButton.vue";
export default {
  name: "YellowButton",
  components: {
    GxButton
  }
};
</script>
