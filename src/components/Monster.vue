<template>
  <div class="monster">
      <BodyPart link="../assets/rubilax/body.jpg"/>
      <BodyPart link="../assets/rubilax/head.jpg"/>
      <BodyPart link="../assets/rubilax/arm-right.jpg"/>
      <BodyPart link="../assets/rubilax/arm-left.jpg"/>
      <BodyPart link="../assets/rubilax/leg-left.jpg"/>
      <BodyPart link="../assets/rubilax/leg-right.jpg"/>
  </div>
</template>

<script>
import BodyPart from './BodyPart.vue'

export default {
  name: 'Monster',
  components: {
      BodyPart
  }
}
</script>

<style scoped>
</style>
