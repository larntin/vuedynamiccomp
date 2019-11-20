<template>
  <div class="code-create">
    <h2>Dynamically inserted:</h2>
    <div ref="container">
      <button @click="onClick">Click to insert</button>
    </div>
  </div>
</template>

<script>
import Vue from "vue";
import Button from "./Button";

export default {
  name: "CodeCreate",
  props: {
    msg: String
  },
  methods: {
    onClick() {
      var ComponentClass = Vue.extend(Button);
      var instance = new ComponentClass({
        propsData: { type: "primary" }
      });
      instance.$slots.default = ["Click me!"];
      // 可以传参挂载到dom节点上
      instance.$mount();
      // 也可以不挂载到任何dom节点上之后这样挂载
      this.$refs.container.appendChild(instance.$el);
    }
  },
  components: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
