<script setup>
// No script needed for static footer
</script>

<template>
  <footer class="bg-gray-900/80 text-gray-300 border-t border-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col md:flex-row justify-between items-center py-6">
        <!-- Left side: branding & ISO badge -->
        <div class="flex items-center space-x-4 mb-4 md:mb-0">
          <span class="text-xl font-bold text-gradient">JUNED</span>
          <span class="inline-flex items-center px-2 py-0.5 rounded bg-emerald-500/10 text-emerald-400 border border-emerald-500/30 text-xs font-medium">
            ISO 27001 Certified
          </span>
        </div>
        <!-- Center: social icons -->
        <div class="flex space-x-4">
          <a href="#" class="text-gray-400 hover:text-cyan-400 transition-colors" aria-label="Twitter">
            <svg class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
              <path d="M23 3a10.9 10.9 0 01-3.14 1.53A4.48 4.48 0 0012.07 8v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2c9 5 20 0 20-11.5a4.5 4.5 0 00-.08-.83A7.72 7.72 0 0024 4.56a7.72 7.72 0 01-2.23.61z"/>
            </svg>
          </a>
          <a href="#" class="text-gray-400 hover:text-violet-400 transition-colors" aria-label="LinkedIn">
            <svg class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
              <path d="M19 0h-14c-2.76 0-5 2.24-5 5v14c0 2.76 2.24 5 5 5h14c2.76 0 5-2.24 5-5v-14c0-2.76-2.24-5-5-5zm-11 19h-3v-10h3v10zm-1.5-11.3c-.97 0-1.75-.79-1.75-1.75s.78-1.75 1.75-1.75 1.75.79 1.75 1.75-.78 1.75-1.75 1.75zm13.5 11.3h-3v-5.5c0-1.31-.03-3-1.84-3-1.84 0-2.13 1.44-2.13 2.9v5.6h-3v-10h2.88v1.36h.04c.4-.74 1.38-1.52 2.84-1.52 3.04 0 3.6 2 3.6 4.6v5.56z"/>
            </svg>
          </a>
        </div>
        <!-- Right side: copyright -->
        <div class="text-sm text-gray-500 mt-4 md:mt-0">
          © {{ new Date().getFullYear() }} JUNED. All rights reserved.
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.text-gradient {
  background: linear-gradient(90deg, #06b6d4, #7c3aed);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>
