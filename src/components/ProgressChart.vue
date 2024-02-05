<template>
  <div class="bg-[#272A32] rounded-xl shadow-lg overflow-hidden max-w-md mx-auto ml-12 text-white">
    <!-- Bagian untuk Total Earning -->
    <div class="flex items-center mb-6 ml-12">
      <!-- Placeholder untuk chart -->

      <div>
        <div
          class="w-24 h-24 bg-blue-300 rounded-full flex items-center justify-center m-3 ml-4 mr-20"
        >
          <!-- Placeholder untuk icon di tengah chart -->
          <div class="bg-blue-500 rounded-full w-10 h-10"></div>
        </div>
        <h3 class="text-sm font-semibold">Total Earning</h3>
        <div class="text-2xl font-bold">$1,837</div>
        <ul class="mt-2 space-y-1">
          <li class="flex items-center">
            <span class="w-2 h-2 bg-green-400 rounded-full mr-4"></span>
            Lorem ipsum +23
          </li>
          <li class="flex items-center">
            <span class="w-2 h-2 bg-blue-400 rounded-full mr-4"></span>
            Ipsum Dolor +34
          </li>
          <li class="flex items-center">
            <span class="w-2 h-2 bg-red-400 rounded-full mr-4"></span>
            Sit Dolor -12
          </li>
        </ul>
      </div>
    </div>

    <!-- Bagian untuk Total Booking -->
    <div class="flex items-center mb-6 ml-12">
      <!-- Placeholder untuk chart -->

      <div>
        <div class="w-24 h-24 bg-blue-300 rounded-full flex items-center justify-center m-3">
          <!-- Placeholder untuk icon di tengah chart -->
          <div class="bg-blue-500 rounded-full w-10 h-10"></div>
        </div>
        <h3 class="text-sm font-semibold">Total Booking</h3>
        <div class="text-2xl font-bold">$2,091</div>
        <ul class="mt-2 space-y-1">
          <li class="flex items-center">
            <span class="w-2 h-2 bg-green-400 rounded-full mr-4"></span>
            Lorem ipsum +23
          </li>
          <li class="flex items-center">
            <span class="w-2 h-2 bg-blue-400 rounded-full mr-4"></span>
            Ipsum Dolor +34
          </li>
          <li class="flex items-center">
            <span class="w-2 h-2 bg-red-400 rounded-full mr-4"></span>
            Sit Dolor -12
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProgressChart'
  // Props and data can be added here if needed for dynamic functionality
}
</script>

<style scoped>
/* Add additional styles if necessary */
</style>
