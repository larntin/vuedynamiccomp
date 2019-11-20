<template>
  <div class="dynamic">
    <div class="github-link">
      同类高级用法：<br>
      <ul>
        <li><a href="https://github.com/larntin/vue-dynamic" target="_blank">https://github.com/larntin/vue-dynamic</a></li>
      </ul>
    </div>
    <component v-for="field in fields" :key="field.id" :is="field.type" v-bind="field"></component>
  </div>
</template>

<script>

import RadioField from '../dynamic-component/RadioField'
import SelectField from '../dynamic-component/SelectField'
import TextField from '../dynamic-component/TextField'

export default {
  name: "dynamicView",
  components: {
    RadioField,
    SelectField,
    TextField
  },
  data() {
    return {
      fields: [
        {
          id: 1,
          label: "Name",
          type: "textField"
        },
        {
          id: 2,
          label: "Email",
          type: "textField"
        },
        {
          id: 3,
          label: "Movies",
          type: "selectField",
          answers: [
            { value: 1, label: "Aa" },
            { value: 2, label: "Bb" },
            { value: 3, label: "Cc" }
          ]
        },
        {
          id: 4,
          label: "Food",
          type: "radioField",
          answers: [
            { value: 1, label: "Aa" },
            { value: 2, label: "Bb" },
            { value: 3, label: "Cc" }
          ]
        }
      ]
    };
  }
};
</script>

<style>
.github-link {
  padding: 10px;
}
</style>
