<template>
  <div id="app" class="flex flex-col bg-tertiary">
    <AppHeader />
    <router-view />
    <AppFooter />
  </div>
</template>

<script setup>
import { ref } from "vue";
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
</script>
