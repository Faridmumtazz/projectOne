<template>
  <div class="bg-blue-500 rounded-xl shadow-lg overflow-hidden max-w-md mx-auto ml-12 text-white">
    <ul>
      <li
        v-for="(item, index) in items"
        :key="index"
        class="py-2 border-b border-blue-300 last:border-b-0 ml-4 mr-4"
      >
        <div class="flex justify-start items-center px-4">
          <div>
            <h3 class="text-sm font-semibold">{{ item.title }}</h3>
            <div class="text-lg font-bold">{{ item.value }}</div>
            <p class="text-xs">{{ item.description }}</p>
          </div>
          <div class="flex items-center space-x-1">
            <span :class="{ 'text-green-400': item.isPositive, 'text-red-400': !item.isPositive }">
              <span v-if="item.isPositive">↑</span>
              <span v-else>↓</span>
            </span>
            <span class="text-sm font-bold">{{ item.percentageChange }}%</span>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'InfoCard',
  props: {
    items: {
      type: Array,
      default: () => []
    }
  }
}
</script>

<style scoped>
/* Tambahkan gaya tambahan jika perlu */
</style>
