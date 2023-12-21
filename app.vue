<script setup lang="ts">
const { data: test } = await useFetch('/api/test')
</script>

<template>
  <div>
    Hello {{ test?.hello }}!
  </div>
</template>
