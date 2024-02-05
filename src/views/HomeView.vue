<template>
  <div class="bg-[#121317] min-h-screen">
    <nav
      class="bg-[#272A32] fixed top-0 left-0 right-0 h-12 flex justify-between items-center px-12 z-10"
    >
      <div class="flex items-center gap-2">
        <!-- Icon Placeholder -->
        <img :src="logo" alt="Logo" class="w-7 h-7" />
        <div class="flex">
          <h1 class="text-white font-normal text-lg">Sygnos</h1>
          <h1 class="text-white font-bold text-lg">FLOW</h1>
        </div>
      </div>
      <div class="relative rounded-full bg-white">
        <!-- Input untuk pencarian -->
        <input
          type="text"
          placeholder="Search"
          class="pl-4 pr-10 py-1 w-full rounded-full text-sm focus:outline-none"
        />
        <!-- Ikon pencarian -->
        <div class="absolute inset-y-0 right-0 flex items-center pr-3 pointer-events-none">
          <img :src="search" alt="Search" class="w-4 h-4" />
        </div>
      </div>
    </nav>

    <main class="pt-2 pb-2 flex flex-start items-start">
      <!-- Anda bisa menambahkan margin atas tambahan jika diperlukan -->

      <div class="mt-14 w-full max-w-2xl flex flex-col gap-6">
        <!-- Menggunakan komponen InfoCard -->
        <InfoCard
          :items="[
            {
              title: 'Purchase lorem',
              value: '$32.37',
              percentageChange: 12,
              description: 'Lorem Ipsum $737 dolor',
              isPositive: true
            },
            {
              title: 'Sales percent',
              value: '$156.7',
              percentageChange: 9,
              description: 'Lorem Ipsum $347 dolor',
              isPositive: false
            },
            {
              title: 'Total earning',
              value: '$12,837',
              percentageChange: 7,
              description: 'Lorem Ipsum $56 dolor lsd',
              isPositive: true
            }
          ]"
        />
        <ProgressChart />
      </div>
      <section class="flex justify-center mt-12">
        <TimeTabs />
      </section>
    </main>
  </div>
</template>

<script>
// Impor gambar secara eksplisit di sini
import logo from '@/assets/images/Logo.png'
import search from '@/assets/images/search.jpeg'

import InfoCard from '@/components/InfoCard.vue'

import ProgressChart from '@/components/ProgressChart.vue'
import TimeTabs from '@/components/TimeTabs.vue'

export default {
  name: 'HomeView',
  components: {
    // Daftarkan komponen InfoCard dan ChartCard
    InfoCard,
    ProgressChart,
    TimeTabs
  },
  data() {
    return {
      // Data untuk gambar
      logo: logo,
      search: search
    }
  }
}
</script>
