<template>
  <NuxtLink :to="`/products/${card.id}`" class="card-container">
    <img :src="require(`@/assets/images/${card.image }`)" alt="" class="image">
  </NuxtLink>
</template>

<script>
export default {
  props: ['card']

}
</script>

<style scoped>
  .card-container {
    width: 24%;
    height: 12.5rem;
    border-radius: 01.5rem;
    overflow: hidden;
    margin-bottom: 1.5rem;
    cursor: pointer;
    object-fit: cover;
  }
  .image {
    object-fit: cover;
    width: 100%;
    height: 100%;
  }
</style>
