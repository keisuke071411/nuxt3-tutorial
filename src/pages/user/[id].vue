<template>
  <h1>Hello {{ path }}</h1>
  <div>
    <button @click="dec">-</button>
    <p>{{ counter }}</p>
    <button @click="inc">+</button>
  </div>
  <NuxtLink to="/">ページ遷移</NuxtLink>
</template>

<script setup lang="ts">
const route = useRoute();

const path = computed(() => route.params.id as string);
const { counter, inc, dec } = useCounter();
</script>

<style lang="scss" scoped>
div {
  display: flex;
  justify-content: center;
  gap: 20px;
}
</style>
