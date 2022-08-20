<script setup>
// Importing things we need
import { ref } from "@vue/reactivity";
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <!-- Container  -->
  <div class="container">
    <!-- Navbar -->
    <Navbar />
    <!-- Router view  -->
    <router-view />
    <!-- Footer  -->
    <Footer />
  </div>
  <!-- Container  -->
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=DynaPuff&family=Lato:wght@400;700&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Lato", sans-serif;
}
</style>

