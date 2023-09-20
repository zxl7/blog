<template>
  <main class="main-home dsbc">
    <aside class="main-item" v-for="(item, index) in dataList" :key="index">
      <img class="item-img" :src="item.imgUrl" alt="" />
      <p class="item-time">{{ item.tags }}・{{ item.updateTime }}</p>
      <h3>{{ item.title }}</h3>
      <p class="item-desc">{{ item.desc }}</p>
    </aside>
  </main>
</template>
<script setup lang="ts">
import images from "@/assets/images/1.jpg"
import { ref } from "vue"
const dataList = ref([
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
  { imgUrl: images, title: "标题1", desc: "描述1", updateTime: "2021-10-01", tags: "标签1, 标签2" },
])
</script>
<style scoped>
.main-home {
  flex-wrap: wrap;
  .main-item {
    width: 30%;
  }
  .item-img {
    width: 100%;
    height: 100%;
    border-radius: 10px;
  }
  .item-time {
    height: 20px;
    font-size: 14px;
    font-weight: normal;
    line-height: 20px;
    letter-spacing: 0px;
    color: #333333;
  }
  .item-desc {
    font-size: 14px;
    font-weight: 250;
    line-height: 28px;
    letter-spacing: 0px;
    color: #333333;
  }
}
</style>
