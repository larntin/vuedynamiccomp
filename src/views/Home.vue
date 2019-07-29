<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <code-create msg="Welcome to Your Vue.js App"></code-create>
  </div>
</template>

<script>
// @ is an alias to /src
import CodeCreate from '@/code-create/CodeCreate'

export default {
  name: 'home',
  components: {
    CodeCreate
  }
}
</script>
