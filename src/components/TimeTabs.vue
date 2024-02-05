<template>
  <div class="flex justify-center items-center bg-[#272A32] rounded-lg p-1 space-x-1">
    <button
      v-for="tab in tabs"
      :key="tab"
      class="px-3 py-1 rounded-lg focus:outline-none transition-colors duration-150"
      :class="[currentTab === tab ? 'bg-white text-[#272A32]' : 'text-white bg-transparent']"
      @click="currentTab = tab"
    >
      {{ tab }}
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentTab: '1W', // Default selected tab
      tabs: ['1H', '1D', '1W', '1M', 'ALL'] // List of tabs
    }
  }
}
</script>

<style scoped>
/* You can add additional styles here */
</style>
