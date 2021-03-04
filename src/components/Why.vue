<template>

  <div style="position: relative">
    <Title title="Why Technotrade" />

    <div class="comp">
      <div class="why-icon">
        <img src="@/assets/w4.png" alt="Trade Across The World">
        <div class="why-text">
          <p>Trade Across <br> The World</p>
        </div>
      </div>
      <div class="why-icon">
        <img src="@/assets/w3.png" alt="Completely Transparent">
        <div class="why-text">
          <p>Completely <br> Transparent</p>
        </div>
      </div>
      <div class="why-icon">
        <img src="@/assets/w2.png" alt="Modelled Around Bussiness">
        <div class="why-text">
          <p>Modelled Around <br> Bussiness</p>
        </div>
      </div>
      <div class="why-icon">
        <img src="@/assets/w1.png" alt="Cost Effective">
        <div class="why-text">
          <p>Cost <br> Effective</p>
        </div>
      </div>

    </div>
  </div>
</template>


<style scoped>


  .why-icon {
    min-width: 50%;
    padding: 2em 0.5em;
    display: inline-block;
    border: 1px solid #e6e6e6;
  }

  @media (max-width: 768px) {
      .why-icon {
    width: 50%;
    padding: 2em 0.5em;
    display: inline-block;
    border: 1px solid #e6e6e6;
  }
  }
</style>

<script>
import Title from "./Title"
export default {
  components: {
    Title
  }
}
</script>