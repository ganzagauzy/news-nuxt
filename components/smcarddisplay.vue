<template>
  <div class="container">
    <h3 class="header">
       {{cardsection.title}}
    </h3>
    <div class="card-container">
      <smcard
        v-for="card in cardsection.cards"
        :key="card.id"
        :card = "card"
      />
    </div>

  </div>
</template>

<script>
import smcard from './smcard.vue'
export default {
  components: { smcard },
  props: ['cardsection']

}
</script>

<style scoped>
  .container {
    padding: 2rem 0;
  }
  .header {
    font-weight: 700;
    font-size: 1.5rem;
    margin-bottom: 2rem;
  }
  .card-container {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
  }

</style>

