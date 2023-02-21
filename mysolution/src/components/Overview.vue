<template>
  <div class="overview-container">
    <div class="head">Your Result</div>
    <div class="circle">
      <div class="hor-center">
        <div class="number">76</div>
        <div class="of-100">of 100</div>
      </div>
    </div>
    <div class="great">Great</div>
    <p class="text">
      You scored higher than 65% of the people
      who have taken these tests.
    </p>
  </div>
</template>

<style scoped>
  .overview-container {
    background: linear-gradient(hsl(252, 100%, 67%), hsl(241, 81%, 54%));
    text-align: center;
    padding: 20px;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
  }

  .head {
    font-weight: 700;
    color: hsl(241, 100%, 89%);
    font-size: medium;
  }

  .circle {
    background: linear-gradient(hsla(256, 72%, 46%, 1), hsla(241, 72%, 46%, 0));
    display: inline-block;
    margin: 12px;
    border-radius: 50px;
    width: 100px;
    color: hsl(0, 0%, 100%);
    height: 100px;
  }

  .number {
    font-weight: 800;
    font-size: xx-large;
  }

  .hor-center {
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 100%;
  }

  .of-100 {
    opacity: .5;
    font-weight: 700;
    font-size: small;
  }

  .great {
    color: white;
    font-weight: 800;
    font-size: large;
  }

  .text {
    color: hsl(241, 100%, 89%);
    font-weight: 500;
    font-size: small;
  }

  @media (min-width: 700px) {
    .overview-container {
      display: block;
      border-radius: 30px;
      width: 50%;
      padding: 40px;
    }

    .head {
      font-size: 18px;
    }

    .circle {
      margin-top: 30px;
      margin-bottom: 30px;
      width: 200px;
      height: 200px;
      border-radius: 100px;
    }

    .number {
      font-size: xxx-large;
    }

    .of-100 {
      font-size: large;
    }

    .great {
      font-size: x-large;
    }

    .text {
      font-size: large;
    }
  }

</style>