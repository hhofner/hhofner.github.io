<script setup lang="ts">
defineProps<{
  type: 'mini' | 'post'
}>()
</script>

<template>
  <div class="container" :class="type">
    {{type}}
  </div>
</template>

<style scoped>
  .container {
    font-size: 0.75rem;
    border-radius: 15%;
    padding: 0 0.5rem;
    width: fit-content;
  }
  .mini {
    background: #f0f030;
    color: #828201;
  }
  .post {
    background: #09a809;
    color: rgb(77, 234, 77);
  }
</style>