<template>
  <div class="bg-blue-500 rounded-lg p-4 text-white shadow-lg">
    <h3 class="text-lg font-semibold">{{ title }}</h3>
    <!-- Tempat untuk grafik batang Anda -->
    <!-- Misalnya, jika Anda menggunakan Chart.js atau library lain, Anda bisa meletakkannya di sini -->
    <!-- Pastikan untuk mengimpor dan menggunakan library grafik yang sesuai -->
  </div>
</template>

<script>
export default {
  name: 'ChartCard',
  props: {
    title: String
    // Props lain untuk data grafik jika diperlukan
  }
}
</script>
