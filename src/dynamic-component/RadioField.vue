<template>
  <div>
    {{ label }}
    <br />
    <div v-for="answer in answers" :key="answer.value">
      {{ answer.label }}
      <input type="radio" :name="id" :value="answer.value" />
    </div>
  </div>
</template>

<script>
export default {
  name: "radioField",
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
