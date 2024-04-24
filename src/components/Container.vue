<script setup>
  import Accordion from './Accordion.vue';
</script>

<template>
  <div class="container">
    <div class="faqs">
      <img src="../assets/images/icon-star.svg" alt="icon-star" />
      <h1>FAQs</h1>
    </div>
    <Accordion />
  </div>
</template>

<style scoped>
  .container {
    margin-top: 20px;
    max-width: 460px;
    width: 90vw;
    min-height: 460px;
    height: fit-content;
    border-radius: 15px;
    padding: 40px 40px;
    background-color: #fff;
  }

  .faqs {
    display: flex;
    gap: 25px;
  }

  h1 {
    font-size: 3.2rem;
  }
</style>