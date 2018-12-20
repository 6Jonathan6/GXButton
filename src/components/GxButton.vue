<template>
  <button @click="onClick" :disabled="isDisabled">
    <slot></slot>
  </button>
</template>
<script>
export default {
  name: "GxButton",
  props: {
    propagate: {
      type: Boolean,
      default: false
    },
    isDisabled: {
      type: Boolean,
      default: false
    }
  },
  methods: {
    onClick() {
      if (this.propagate) {
        this.$parent.$emit("click");
      } else {
        this.$emit("click");
      }
    }
  }
};
</script>
