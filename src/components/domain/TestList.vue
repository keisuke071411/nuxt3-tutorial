<template>
  <div>
    <p>id: {{ num }}</p>
    <p>name: {{ name }}</p>
    <p>tag: {{ tag }}</p>
  </div>
</template>

<script setup lang="ts">
interface Props {
  name: string;
  num: number;
  tag: string[];
}

const { name, num, tag } = defineProps<Props>();
</script>
