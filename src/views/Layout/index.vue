<script setup>
import LayoutNav from "@/views/Layout/componenents/LayoutNav.vue";
import LayoutHeader from "@/views/Layout/componenents/LayoutHeader.vue";
import LayoutFooter from "@/views/Layout/componenents/LayoutFooter.vue";
</script>

<template>
  <LayoutNav />
  <LayoutHeader />
  <LayoutFooter />
  <RouterView />
</template>
