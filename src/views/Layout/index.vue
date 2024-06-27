<script setup>
import LayoutNav from "@/views/Layout/componenents/LayoutNav.vue";
import LayoutHeader from "@/views/Layout/componenents/LayoutHeader.vue";
import LayoutFooter from "@/views/Layout/componenents/LayoutFooter.vue";
import LayoutFixed from "@/views/Layout/componenents/LayoutFixed.vue";

//触发获取导航列表的action
import { useCategoryStore } from "@/stores/categoryStore";
import { onMounted } from "vue";
const CategoryStore = useCategoryStore();

onMounted(() => CategoryStore.getCategory());
</script>

<template>
  <LayoutNav />
  <LayoutFixed />
  <LayoutHeader />
  <!-- 添加key 破坏复用机制 强制销毁重建 -->
  <!-- <RouterView :key="$route.fullPath" /> -->
  <RouterView />
  <LayoutFooter />
</template>
