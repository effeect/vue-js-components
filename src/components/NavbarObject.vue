<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="#">
        <!-- Logo or brand name -->
        <strong>Oliver James Dimes</strong>
      </a>

      <!-- Burger menu for mobile -->
      <a
        role="button"
        class="navbar-burger"
        :class="{ 'is-active': isActive }"
        aria-label="menu"
        aria-expanded="false"
        @click="toggleMenu"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div class="navbar-menu" :class="{ 'is-active': isActive }">
      <div class="navbar-end">
        <a class="navbar-item" href="#">Item #1</a>
        <a class="navbar-item" href="#">Item #2</a>
        <a class="navbar-item" href="#">Item #3</a>
      </div>
    </div>
  </nav>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const isActive = ref(false)

const toggleMenu = () => {
  isActive.value = !isActive.value
}
</script>

<style scoped>
/* Optional: tweak spacing or colors */
.navbar-item strong {
  font-size: 1.2rem;
}
.navbar-item:hover {
  font-size:;
  color: white;
}
</style>
