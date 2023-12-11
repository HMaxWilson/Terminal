<script setup>
import { RouterView } from 'vue-router'
import Overlay from './components/global/TheOverlay.vue'
import Header from './components/global/TheHeader.vue'
import Navbar from './components/global/TheNavbar.vue'
</script>

<template>
  <Overlay />
  <div class="wrapper">
    <div class="content clearfix">
      <Header />
      <Navbar />

      <main>
        <RouterView v-slot="{Component}">
          <transition name="fade" mode="out-in">
            <component :is="Component" :key="$route.path" />
          </transition>
        </RouterView>
      </main>
    </div>
  </div>
</template>

<style>
.wrapper {
  animation: scroll 5s 1;
  margin: 0;
  padding: 0;
}

.content {
  animation: scroll 3s 1;
  overflow: hidden;
  padding: 40px;
  position: relative;
  width: 95%;
  margin: 0 auto;
}

@keyframes scroll {
  0% { height: 0 }
  100% { height: 100%; }
}

.fade-enter-active, .fade-leave-active {
  transition: opacity 0.8s;
}
.fade-enter-from, .fade-leave-to {
  opacity: 0;
}

@media screen and (max-width: 768px) {
  .content {
    padding: 10px;
  }
}
</style>