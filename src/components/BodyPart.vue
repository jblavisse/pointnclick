<template>
  <div class="body-part">
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
