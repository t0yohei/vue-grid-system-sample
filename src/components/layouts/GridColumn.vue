<script setup lang="ts">
type Props = {
  pc: 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12
}

defineProps<Props>()
</script>

<template>
  <div class="grid-colomn">
    <slot />
  </div>
</template>

<style scoped>
.grid-colomn {
  grid-column: auto/span v-bind(pc); /* 開始位置は auto で pc に指定された値分伸ばす */
}
</style>
