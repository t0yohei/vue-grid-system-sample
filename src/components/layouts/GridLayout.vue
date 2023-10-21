<template>
  <div class="grid-layout">
    <slot />
  </div>
</template>

<style scoped>
.grid-layout {
  display: grid;
  grid-template-columns: repeat(12, 1fr); /* 12 分割を指定 */
}
</style>
