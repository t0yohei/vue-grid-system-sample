<script setup lang="ts">
type ColumnNum = 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12
type Props = {
  pc: ColumnNum
  tbl: ColumnNum
  sp: ColumnNum
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

@media screen and (width < 1200px) {
  .grid-colomn {
    grid-column: auto/span v-bind(tbl); /* 開始位置は auto で tbl に指定された値分伸ばす */
  }
}

@media screen and (width < 576px) {
  .grid-colomn {
    grid-column: auto/span v-bind(sp); /* 開始位置は auto で sp に指定された値分伸ばす */
  }
}
</style>
