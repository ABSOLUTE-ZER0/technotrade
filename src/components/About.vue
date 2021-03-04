<template>
  <div class="about comp">
    <h3 class="about-heading">What Is Technotrade</h3>
    <p class="about-text">Some random Text.</p>
    <b-button href="#" variant="info">Read More</b-button>
  </div>
</template>

<style scoped>
  .about-heading {
    font-size: 1.5em;
    text-transform: uppercase;
    color: #343434;
  }

  .about-text {
    font-size: 1em;
    width: 100%;
    float: left;
    position: relative;
    color: #343434;
    padding-left: 1.5em;
    padding-right: 1.5em;
  }

  .about {
    text-align: center;
    width: 100%;
    position: relative;
    background-color: #fff;
    border: 1px solid #e6e6e6;
    padding: 1em 0;
  }

  @media (max-width: 768px) {
      .about {
    margin: 0 -15px -15px 0;
  }

    .about-heading {
    font-size: 1.1em;
    font-weight: 500;
  }

  }
</style>