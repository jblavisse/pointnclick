<template>
  <div class="boss">
      <img src="../assets/rushu.png" alt="THE BOSS">
      <h2>Rushu</h2>
      <div>
          <span class="remaining-points">{{remainingPoints}}</span>
          <span class="life-points">/{{lifePoints}}</span>
     </div>
  </div>
</template>

<script>
export default {
  name: 'Boss',
  computed:{
      remainingPoints: function()
      {
          return this.$root.$data.store.remainingPoints;
      },
      lifePoints: function()
      {
         return  this.$root.$data.store.lifePoints;
      }
  },
}
</script>

<style scoped>
span {
    font-size: 2rem;
}
</style>
