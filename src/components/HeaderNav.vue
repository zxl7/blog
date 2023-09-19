<template>
  <header class="header dfsc">
    <span class="header-title">逆水行舟丨⛵️</span>
    <nav class="header-nav ml_48">
      <RouterLink class="nav-item" to="/">主页</RouterLink>
      <RouterLink class="nav-item" to="/">项目</RouterLink>
      <RouterLink class="nav-item" to="/about">About</RouterLink>
    </nav>
  </header>
</template>
<script lang="ts">
import { defineComponent } from "vue"
import { ref } from "vue"
export default defineComponent({
  name: "HeaderNav",
})
</script>
<style scoped lang="less">
.header {
  padding: 50px 6% 0;

  .header-title {
    font-size: 32px;
  }
  .header-nav {
    .nav-item {
      font-size: 18px;
      margin-left: 24px;
      font-style: normal;
      text-decoration: auto;
      color: #000;
    }
  }
}
</style>
