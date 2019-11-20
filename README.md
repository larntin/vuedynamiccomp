# vuedynamiccomp

# JSX
https://github.com/vuejs/jsx 用于在 Vue 中使用 JSX 语法，它可以让我们回到更接近于模板的语法上。

将 h 作为 createElement 的别名是 Vue 生态系统中的一个通用惯例，实际上也是 JSX 所要求的。从 Vue 的 Babel 插件的 3.4.0 版本开始，我们会在以 ES2015 语法声明的含有 JSX 的任何方法和 getter 中 (不是函数或箭头函数中) 自动注入 const h = this.$createElement，这样你就可以去掉 (h) 参数了。对于更早版本的插件，如果 h 在当前作用域中不可用，应用会抛错。

## JSX安装

npm install @vue/babel-preset-jsx @vue/babel-helper-vue-jsx-merge-props

Then add the preset to .babelrc:
{
  "presets": ["@vue/babel-preset-jsx"]
}

## Vue JSX的兼容性
Babel 7+. For Babel 6 support, use `vuejs/babel-plugin-transform-vue-jsx`
Vue 2+. JSX is not supported for older versions.
