<script>
export default {
  render: function(createElement) {
    // render 函数的通用写法，使用 createElement 来编写每一个内部渲染标签
    // createElement 2个参数的时候，第二个参数是子组件数组VNode[]
    return createElement(
      "h" + this.level,     // 标签名称
      this.$slots.default   // 子节点数组
    );
  },
  props: {
    level: {
      type: Number,
      required: true
    }
  }
};
</script>
