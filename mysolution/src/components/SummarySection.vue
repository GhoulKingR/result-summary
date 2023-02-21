<script setup>
  import SummaryItem from './SummaryItem.vue';
  import ContinueButton from './ContinueButton.vue';
  
  let data = `[
    {
      "category": "Reaction",
      "score": 80,
      "icon": "./assets/images/icon-reaction.svg"
    },
    {
      "category": "Memory",
      "score": 92,
      "icon": "./assets/images/icon-memory.svg"
    },
    {
      "category": "Verbal",
      "score": 61,
      "icon": "./assets/images/icon-verbal.svg"
    },
    {
      "category": "Visual",
      "score": 72,
      "icon": "../assets/images/icon-visual.svg"
    }
  ]
  `;
  let object = JSON.parse(data);
</script>

<template>
  <div class="container">
    <div class="text">Summary</div>
    <SummaryItem :data="object[0]" style="background-color: hsla(0, 100%, 67%, .1); color: hsl(0, 100%, 67%);"/>
    <SummaryItem :data="object[1]" style="background-color: hsla(39, 100%, 56%, .1); color: hsl(39, 100%, 56%);"/>
    <SummaryItem :data="object[2]" style="background-color: hsla(166, 100%, 37%, .1); color: hsl(166, 100%, 37%);"/>
    <SummaryItem :data="object[3]" style="background-color: hsla(234, 85%, 45%, .1); color: hsl(234, 85%, 45%);"/>
    <ContinueButton />
  </div>
</template>

<style scoped>
  .container {
    padding: 20px;
  }

  .text {
    color: hsl(224, 30%, 27%);
    font-weight: 700;
    margin-bottom: 20px;
  }
</style>