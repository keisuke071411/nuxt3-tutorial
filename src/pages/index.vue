<template>
  <h1>hello world</h1>
  <p>{{ counter }}</p>
  <NuxtLink to="/test">ページ遷移</NuxtLink>
</template>

<script setup lang="ts">
const { counter } = useCounter();
</script>
