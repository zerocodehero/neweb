<template>
  <div></div>
</template>

<script setup>
import { ref } from 'vue'
const count = ref(0)
if (count.value !== 0) {
    console.log('foo')
}

</script>

<style lang="scss" scoped></style>