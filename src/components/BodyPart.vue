<template>
  <div class="body-part" @click="removeOnePoint">
      <img :src="require(`@/assets/rubilax/${link}`)" alt="Sous-fifre">
      <div :class="position">
          <span class="remaining-points">{{remainingPoints}}</span>
          <span class="life-points">/{{lifePoints}}</span>
     </div>
  </div>
</template>

<script>

export default {
  name: 'BodyPart',
  props: ['link','position'],
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
  methods: {
      removeOnePoint: function()
      {
          this.$root.$data.store.remainingPoints--;
          console.log(this.$root.$data.store.remainingPoints)
      }
  }
}
</script>

<style scoped>
span {
    font-size: 0.75rem;
}

img {
    cursor:pointer;
}

.body-part {
    position: relative;
}

.center {
    position: absolute;
    top: 200px;
    left: 140px;
    z-index: 4;
}

.top {
    position: absolute;
    left: 200px;
    top: 0px;
}

.top-left {
    position: absolute;
    left: 300px;
    top: 30px;
}

.top-right {
    position: absolute;
    left: 100px;
    top: 30px;
}

.bottom-left {
    position: absolute;
    left: 300px;
    top: 280px;  
}

.bottom-right {
    position: absolute;
    left: 100px;
    top: 280px;  
}
</style>
