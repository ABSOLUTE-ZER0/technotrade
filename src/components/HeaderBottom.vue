<template>
  <div class="header-bottom">
    <b-navbar toggleable="lg">
      <b-navbar-brand class="nav-item" href="#">
        <img src="@/assets/msg.png" class="d-inline-block brand-img align-top" alt="Kitten">
        TechnoTrade
      </b-navbar-brand>
      <b-navbar-nav class="ml-auto">
        <b-nav-item class="nav-item" href="#">About Us
        </b-nav-item>
        <b-nav-item class="nav-item" href="#">Products
        </b-nav-item>
        <b-nav-item class="nav-item" href="#">How It Works
        </b-nav-item>
        <b-nav-item class="nav-item" href="#"> Why Technotrade</b-nav-item>
        <b-nav-item class="nav-item" href="#"> Contact Us</b-nav-item>
        <b-nav-item class="nav-item" href="#"> Branded Solution</b-nav-item>
        <b-nav-item class="nav-item" href="#"> Media</b-nav-item>
        <b-button class="signin-btn">GET A QUOTE</b-button>
        <b-button class="seach-btn">
          <b-icon icon="search"></b-icon>
        </b-button>
      </b-navbar-nav>
    </b-navbar>
  </div>
</template>

<style scoped>
  .nav-item {
    margin: 0 1em;

  }

  .brand-img {
    width: 2em;
  }

  .header-bottom {
    background-color: rgb(0, 204, 255);
    font-size: 0.9em;
    padding: 0.5em 10%;

  }


  .signin-btn {
    font-weight: bold;
    background-color: orangered;
    font-size: 0.9em;
    border: 0;
  }

  .seach-btn {
    background-color: rgb(0, 204, 255);
    border: 0;
    color: black;
  }
</style>