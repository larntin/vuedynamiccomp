<script>
import AnchoredHeading from "../jsx-render/AnchoredHeading.vue";

export default {
  components: { AnchoredHeading },

  // 将 h 作为 createElement 的别名是 Vue 生态系统中的一个通用惯例
  // 这样写是最小的可以生效的写法，当前版本中这个 h 参数不能生，省略会出错
  render: h => (
    <AnchoredHeading level={1}>
      <span>Hello</span> world!
    </AnchoredHeading>
  )
};
</script>
