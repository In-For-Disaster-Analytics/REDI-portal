<template>
  <div class="button-counter">
    <button @click="count++">You clicked me {{ count }} times.</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<style lang="scss">
.button-counter {
  width: 300px;
  height: 150px;
  background-color: orange;
}
</style>
