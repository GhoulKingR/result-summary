<script setup>
  import Overview from './components/Overview.vue';
  import SummarySection from './components/SummarySection.vue';
</script>

<template>
  <div class="center-ver">
    <div class="center-hor">
      <div class="container">
        <Overview/>
        <SummarySection/>
      </div>
    </div>
  </div>
</template>

<style scoped>
  @media (min-width: 700px) {
    .center-ver {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .center-hor {
      width: 100vw;
      display: flex;
      justify-content: center;
    }
    .container {
      display: flex;
      width: 700px;
      border-radius: 30px;
      box-shadow: 10px 10px 20px rgb(215, 215, 215);
    }
  }
</style>
