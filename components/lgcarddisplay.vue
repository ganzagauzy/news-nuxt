<template>
  <div class="container">
    <div>
      <h4 class="header">
        {{cardssection.title}}
      </h4>
      <p class="snippet">
        {{cardssection.snippet}}
      </p>
    </div>

    <div class="cards-container">
      <lgcard
        v-for="card in cardssection.cards"
        :key="card.id"
        :card = "card"
      />

    </div>
  </div>
</template>

<script>
export default {
  props: ['cardssection']

}
</script>

<style scoped>

  .header {
    display: flex;
    justify-content: center;
    margin-top: 100px;
    font-weight: 700;
    font-size: 1.5rem;
  }
  .snippet {
    display: flex;
    justify-content: center;
    color: grey;
    margin-bottom: 1rem;

  }
  .cards-container {
    display: flex;
    justify-content: space-between;
  }

</style>
