<template>
  <footer class="footer">
    <div class="content has-text-centered">
      <p>
        Built with <a href="https://bulma.io/">Bulma</a>. Created on
        <span v-text="createdOn"></span>
      </p>
    </div>
  </footer>
</template>
<script setup lang="ts">
import { ref } from 'vue'

const createdOn = ref(new Date().toLocaleString())
</script>
<style></style>
