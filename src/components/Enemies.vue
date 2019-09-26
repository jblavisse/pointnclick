<template>
  <div class="enemies">
      <Boss/>
      <Monster/>
      <Monster/>
      <Monster/>
  </div>
</template>

<script>
import Boss from './Boss.vue'
import Monster from './Monster.vue'

export default {
  name: 'Enemies',
  components: {
      Boss, 
      Monster
  }
}
</script>

<style scoped>
</style>
