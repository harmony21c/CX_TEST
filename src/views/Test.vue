<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <section class="test-page">
    <h1>Test 페이지</h1>
    <p>이 화면은 <code>/test</code> URL로 접근합니다.</p>
    <button type="button" @click="count++">클릭: {{ count }}</button>
  </section>
</template>

<style scoped>
.test-page {
  padding: 2rem;
  text-align: center;
}

h1 {
  margin-bottom: 0.5rem;
}

p {
  margin-bottom: 1.5rem;
  color: #64748b;
}

button {
  padding: 0.6rem 1.2rem;
  font-size: 1rem;
  cursor: pointer;
}
</style>
