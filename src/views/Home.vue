<template>
  <div class="home">
    <code-create></code-create>
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
