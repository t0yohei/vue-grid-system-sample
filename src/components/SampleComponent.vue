<script setup lang="ts">
import GridLayout from './layouts/GridLayout.vue'
import GridColumn from './layouts/GridColumn.vue'
</script>

<template>
  <GridLayout>
    <GridColumn :pc="4">
      <div class="area">Area 1</div>
    </GridColumn>
    <GridColumn :pc="4">
      <div class="area">Area 2</div>
    </GridColumn>
    <GridColumn :pc="4">
      <div class="area">Area 3</div>
    </GridColumn>
    <GridColumn :pc="4">
      <div class="area">Area 4</div>
    </GridColumn>
    <GridColumn :pc="4">
      <div class="area">Area 5</div>
    </GridColumn>
    <GridColumn :pc="4">
      <div class="area">Area 6</div>
    </GridColumn>
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
