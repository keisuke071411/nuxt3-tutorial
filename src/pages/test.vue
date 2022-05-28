<template>
  <h1>hello test</h1>
  <TestList :name="testList.name" :tag="testList.tag" :num="testList.num" />
  <button>テストボタン</button>
</template>

<script setup lang="ts">
import TestList from "~/components/domain/TestList.vue";

const testList = ref({
  name: "テスト１",
  tag: ["天才", "最高", "きしょい"],
  num: 11
});
</script>
