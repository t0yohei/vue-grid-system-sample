<script setup lang="ts">
import GridLayout from './layouts/GridLayout.vue'
</script>

<template>
  <GridLayout>
    <div class="area">Area 1</div>
    <div class="area">Area 2</div>
    <div class="area">Area 3</div>
    <div class="area">Area 4</div>
    <div class="area">Area 5</div>
    <div class="area">Area 6</div>
  </GridLayout>
</template>

<style scoped>
.area {
  background-color: lightblue;
  height: 40px;
  line-height: 40px;
  text-align: center;
  border: 1px solid;
  text-wrap: nowrap;
  padding: 0 4px;
}
</style>
