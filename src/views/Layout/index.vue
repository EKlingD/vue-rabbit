<script setup>
import LayoutNav from "@/views/Layout/componenents/LayoutNav.vue";
import LayoutHeader from "@/views/Layout/componenents/LayoutHeader.vue";
import LayoutFooter from "@/views/Layout/componenents/LayoutFooter.vue";
import LayoutFixed from "@/views/Layout/componenents/LayoutFixed.vue";
</script>

<template>
  <LayoutFixed />
  <LayoutNav />
  <LayoutHeader />
  <LayoutFooter />
  <RouterView />
</template>
