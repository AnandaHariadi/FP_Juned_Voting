<template>
  <div class="relative rounded-xl bg-white/10 backdrop-blur-md border border-white/20 shadow-lg p-6 overflow-hidden">
    <!-- Glass effect overlay -->
    <div class="absolute inset-0 rounded-xl bg-gradient-to-br from-white/5 via-white/10 to-white/5 pointer-events-none"></div>
    <div class="relative z-10">
      <slot />
    </div>
  </div>
</template>

<script setup lang="ts">
// No props needed – this is a generic container.
</script>

<style scoped>
/* Optional subtle animation when hovered */
div:hover {
  transform: translateY(-2px);
  transition: transform 0.2s ease;
}
</style>
