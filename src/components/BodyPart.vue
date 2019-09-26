<template>
  <div class="body-part">
      <img :src="link" alt="Sous-fifre">
      <h2>Sous-fifre</h2>
      <div>
          <span class="remaining-points">{{remainingPoints}}</span>
          <span class="life-points">/{{lifePoints}}</span>
     </div>
  </div>
</template>

<script>
export default {
  name: 'BodyPart',
  props: ['link'],
  data: function()
  {
      return {
          lifePoints: 50,
          remainingPoints: 50
      }
  }
}
</script>

<style scoped>
span {
    font-size: 0.75rem;
}
</style>
