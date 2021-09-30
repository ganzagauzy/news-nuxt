<template>
  <div class="hero container">
    <div class="text-container">
      <h1 class="header"> Find Your Fire Extinguisher</h1>
      <p class="snippet">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit.
          Nam vero enim minus. Ipsa, necessitatibus delectus!
      </p>
      <button class="button btn">Start Looking</button>
    </div>
    <img src="../assets/svg/fire-extinguisher.svg" alt="" class="image">

  </div>
</template>

<script>

export default {
}
</script>

<style scoped>
  .hero {
      height: 50vh;
      position: relative;
      display: flex;
      padding: 3rem 0;
      align-items: flex-start;
      justify-content: space-between;
      margin-bottom: 10rem;
      margin-top: 1rem;
    }
  .text-container {
        width: 50%;
        margin-top: 1rem;
    }
  .header {
        font-weight: 900;
        font-size: 3rem;
    }
  .snippet {
        color: grey;
        font-size: 1.25rem;
    }
  .image {
        width: 20.5rem;
        margin-top: 2rem;
    }
  .overlay {
        background: rgba(0, 0, 0, 0);
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
    }
  .button {
        padding: 1rem 3rem;
        border-radius: 100rem;
        background-color: rgb(231, 81, 43);
        color: white;
        width: 15rem;
        font-weight: 700;
        transition: 0.5s;
    }
  .button:hover {
        width: 16.5rem;
    }
  @media (max-width: 500px) {
        .hero {
            height: 40vh;


        }
    }
</style>
