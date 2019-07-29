<template>
  <div>
    {{ label }}
    <select :id="id">
      <option v-for="answer in answers" :key="answer.value" :value="answer.value">{{answer.label}}</option>
    </select>
  </div>
</template>

<script>
export default {
  name: "selectField",
  data() {
    return {};
  },
  computed: {},
  props: ["label", "id", "answers"]
};
</script>

<style scoped>
button.primary {
  background: blue;
  color: white;
}
</style>
