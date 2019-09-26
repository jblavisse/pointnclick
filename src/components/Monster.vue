<template>
  <div class="monster">
      <div class="parts">
      <BodyPart link="body.png" position="center" class="part body"/>
      <BodyPart link="leg-left.png" position="bottom-left" class="part leg-left" />
      <BodyPart link="arm-right.png" position="top-right" class="part arm-right" />
      <BodyPart link="arm-left.png" position="top-left"  class="part arm-left" />
      <BodyPart link="leg-right.png" position="bottom-right" class="part leg-right" />
      <BodyPart link="head.png" position="top" class="part head" />
      </div>

      <h2>Sous-fifre</h2>
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
 .parts {
     display: flex;
     position: relative;
 }

.head, .leg-left, .leg-right, .arm-left, .arm-right {
    position: absolute;
    z-index:2;
 }

 .body {
     z-index:1;
 }
 
</style>
