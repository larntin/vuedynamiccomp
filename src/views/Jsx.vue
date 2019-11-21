<template>
  <div class="jsx">
    <div class="github-link">
      同类用法例举：
      <br />
      <li>
        <a
          href="https://github.com/larntin/vue-datasource"
          target="_blank"
        >https://github.com/larntin/vue-datasource</a>
      </li>
    </div>
    <div class="jsx-view">
      <anchored-heading level="3">render 函数通用写法</anchored-heading>
      <anchored-heading level="1">---H1---</anchored-heading>
    </div>
    <div class="jsx-view">
      <j-s-x-render></j-s-x-render>
    </div>
  </div>
</template>

<script>
import AnchoredHeading from "../jsx-render/AnchoredHeading.vue";
import JSXRender from "../jsx-render/JSXRender.vue";
export default {
  name: "jsxView",
  components: { AnchoredHeading, JSXRender },
  data() {
    return {};
  }
};
</script>

<style>
.jsx-view {
  margin-top: 10px;
  width: 100%;
  height: 120px;
  border: 1px solid #ccc;
}
</style>
