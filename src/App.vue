<template>
  <main class="app">
    <HeaderNav />
    <aside class="app-content">
      <RouterView />
    </aside>
  </main>
</template>

<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router"
import HeaderNav from "./components/HeaderNav.vue"
</script>

<style scoped lang="less">
.app {
  width: 70vw;
  background: rgba(255, 255, 255, 0.8);
  min-height: calc(100vh - 48px);
  border-radius: 4px;
  margin: 0 auto;
}
.app-content {
  padding: 40px 10% 0;
  height: calc(100vh - 193px);
  overflow: scroll;
}
canvas {
  display: block;
}
</style>
