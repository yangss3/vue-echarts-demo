<template>
  <PieChart 
    :height="300"
    :width="400"
    bordered
    :series="{
      data: [
        { name: 'China', value: 49 },
        { name: 'USA', value: 69 },
        { name: 'Japan', value: 29 },
        { name: 'Russia', value: 39 }
      ]
    }"
  />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { PieChart } from '@yangss/vue-echarts'

export default defineComponent({
  name: 'App',
  components: {
    PieChart
  }
})
</script>

<style>
#app {
  height: 100vh;
}
</style>
