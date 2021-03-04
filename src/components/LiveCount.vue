<template>
  <b-row class="live-count comp">

    <div class="live-common">
      <div class="live-img">
        <img src="@/assets/live.png" alt="live">
      </div>
      <div class="live-text">
        <h3 class="live-text">Registered<br>Agri Buyers</h3>
      </div>
    </div>

    <div class="live-common">
      <div class="live-img">
        <img src="@/assets/nego.png" alt="nego">
      </div>
      <div class="live-text">
        <h3 class="live-text">Registered<br>Construction Buyers</h3>
      </div>
    </div>

    <div class="live-common">
      <div class="live-img">
        <img src="@/assets/order.png" alt="order">
      </div>
      <div>
        <h3 class="live-text">Registered<br>Sellers</h3>
      </div>
    </div>

  </b-row>
</template>

<style scoped>
  .live-common {
    width: 33.33%;
    display: flex;
    padding: 1em;
    border: 1px solid #e6e6e6;
  }

  .live-text {
    font-size: 0.9em;
    color: grey;
    text-align: left;
    margin: 0.1em;
  }

  .live-count {
    display: flex;
    height: 100%;

  }

  @media (max-width: 768px) {

  .live-common {
    display: block;
  }

    .live-text {
    font-size: 0.9em;
    color: grey;
    text-align: center;
    margin: 0.1em;
  }

    .live-count{
      margin: 0 -15px 1em;
    }

  }


</style>