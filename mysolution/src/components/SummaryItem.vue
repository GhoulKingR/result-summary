<script setup>
  defineProps({
    data: {
      type: Object,
      required: true,
    }
  })
</script>

<template>
  <div class="summary-item-container">
    <div>
      <img :src="data.icon" />
      {{ data.category }}
    </div>

    <div style="color: hsl(224, 30%, 27%);">
      <b>{{ data.score }}</b>
      <span> / 100</span>
    </div>
  </div>
</template>

<style scoped>
  .summary-item-container {
    padding: 20px;
    margin-top: 15px;
    margin-bottom: 15px;
    border-radius: 10px;
    display: flex;
    justify-content: space-between;
    font-size: medium;
    font-weight: 700;
  }

  img {
    vertical-align: top;
    margin-right: 4px;
  }

  span {
    opacity: .5;
  }
</style>