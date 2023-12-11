<script setup>
import { RouterView } from 'vue-router'
import Overlay from './components/global/TheOverlay.vue'
import Header from './components/global/TheHeader.vue'
import Footer from './components/global/TheFooter.vue'
import Navbar from './components/global/TheNavbar.vue'
</script>

<template>
  <Overlay />
  <div class="wrapper">
    <div class="content clearfix">
      <Header />
      <Navbar />

      <main class="container mx-auto pt-10 px-12 text-black text-center">
        <RouterView />
      </main>

      <Footer />
    </div>
  </div>
</template>

<style scoped>
.wrapper {
  animation: scroll 5s 1;
  margin: 0;
  overflow: hidden;
  padding: 0;
  scrollbar-width: none;
  -ms-overflow-style: none;
}

.content {
  animation: scroll 3s 1;
  overflow: hidden;
  padding: 40px;
  position: relative;
  width: 95%;
}

@keyframes scroll {
  0% { height: 0 }
  100% { height: 100%; }
}
</style>