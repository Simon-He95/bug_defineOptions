<script setup lang="ts">
import { ref } from 'vue'

let str = 'hello'
const fun = () => {
  return (str += ' world!')
}

let str2 = 'hello'
const fun2 = () => {
  return (str2 += ' world!')
}
</script>

<template>
  <div>
    <Button>{{ fun() }}</Button>
  </div>
  -------------origin----------
  <div>
    <button>{{ fun2() }}</button>
  </div>
</template>

<style scoped>
</style>
