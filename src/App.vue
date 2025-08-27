<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import MobileMenu from "./components/MobileMenu.vue";
</script>

<template>
  <Header class="hidden md:block" />
  <MobileMenu class="md:hidden" />
  <RouterView />
  <Footer />
</template>
