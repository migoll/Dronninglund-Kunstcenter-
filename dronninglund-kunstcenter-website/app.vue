<template>
  <div>
    <TheHeader />
    <RouterView />
    <TheFooter />
  </div>
</template>

<script setup>
import { RouterView } from "vue-router";
import TheFooter from "./components/the-footer.vue";
import TheHeader from "./components/the-header.vue";
</script>
