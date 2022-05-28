<template>
  <Header />
  <main>
    <slot />
  </main>
  <Footer />
</template>

<script setup lang="ts">
import Header from "~/components/shared/Header.vue";
import Footer from "~/components/shared/Footer.vue";
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}

:root {
  font-size: 10px;
}

li {
  list-style: none;
}

a {
  text-decoration: none;
}

main {
  width: 100%;
  height: 100vh;
}
</style>
