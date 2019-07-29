<template>
  <button :class="type">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "Button",
  props: ["type"]
};
</script>

<style scoped>
button.primary {
  background: blue;
  color: white;
}
</style>
