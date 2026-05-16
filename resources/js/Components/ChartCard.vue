<script setup>
import { defineProps } from 'vue';
import { Bar } from 'vue-chartjs';
import { Chart as ChartJS, BarElement, CategoryScale, LinearScale, Tooltip, Legend } from 'chart.js';

ChartJS.register(BarElement, CategoryScale, LinearScale, Tooltip, Legend);

const props = defineProps({
  chartData: { type: Object, required: true },
  chartOptions: { type: Object, default: () => ({ responsive: true, maintainAspectRatio: false }) },
  title: { type: String, default: '' },
});
</script>

<template>
  <div class="bg-white/10 backdrop-blur-lg rounded-xl border border-white/20 p-4 shadow-md">
    <h3 v-if="title" class="text-lg font-semibold text-white mb-3">{{ title }}</h3>
    <div class="h-48">
      <Bar :data="chartData" :options="chartOptions" />
    </div>
  </div>
</template>

<style scoped>
/* No extra CSS needed – Tailwind provides styling */
</style>
