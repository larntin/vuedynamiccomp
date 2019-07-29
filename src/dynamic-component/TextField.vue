<template>
  <div>
    {{label}}
    <input type="text" :id="id" />
  </div>
</template>

<script>
export default {
  name: "textField",
  data() {
    return {};
  },
  computed: {},
  props: ["label", "id"]
};
</script>

<style scoped>
button.primary {
  background: blue;
  color: white;
}
</style>
