<template>
  <div class="monster">
      <div class="parts">
      <BodyPart link="https://framapic.org/CTkAtE1gURRy/k0yZXPxB9mKU.jpg"/>
      <BodyPart link="https://framapic.org/zPPNREIKAK4X/BhdukoYQcWab.jpg"/>
      <BodyPart link="https://framapic.org/ZHAQ9BSycs8D/lYCXUR0YcTPZ.jpg"/>
      <BodyPart link="https://framapic.org/krZf0nk0XFg5/iWlCGdjWJJ3H.jpg"/>
      <BodyPart link="https://framapic.org/sF5LMLpmsxgk/mYkj8glZHR2w.jpg"/>
      <BodyPart link="https://framapic.org/sF5LMLpmsxgk/mYkj8glZHR2w.jpg"/>
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
 }
</style>
