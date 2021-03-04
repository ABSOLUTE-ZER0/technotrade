<template>
  <div class="header-bottom">
    <b-navbar class="d-none d-lg-flex" toggleable="lg">
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

    <b-navbar class="d-lg-none nav-bar" toggleable="lg">
      <b-navbar-brand class="nav-item nav-brand" href="#">
        <img src="@/assets/msg.png" class="d-inline-block brand-img align-top" alt="Kitten">
        TechnoTrade
      </b-navbar-brand>
      <b-navbar-toggle class="toggle-btn" target="nav-collapse"></b-navbar-toggle>

      <b-collapse style="text-align: center;width:100%" id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/msg.png"> info@technotrade.com
          </b-nav-item>
          <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/call.png"> +91 99999 99999
          </b-nav-item>
          <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/mobile.png"> Download App
          </b-nav-item>
          <b-nav-item class="nav-item" href="#"> Sell on Technotrade</b-nav-item>
          <b-nav-item class="nav-item" href="#"> Careers</b-nav-item>
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
      </b-collapse>
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
    margin: 0.5em 0;
    padding: 0 10%;

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
    margin-left: auto;
  }

  @media (max-width: 1000px) and (min-width: 768px) {}

  @media (max-width: 768px) {
    .nav-item {
      width: 100%;
    }

    .nav-bar {
      width: 100%;
      text-align: left;
      padding: 0 0.5em;
    }

    .toggle-btn {
      margin-left: auto;
    }

    .header-bottom {
      background-color: rgb(0, 204, 255);
      font-size: 0.9em;
      margin: 1em 0 0;
      padding: 0;
    }

    .navtop-img {
      width: 1em;
      margin-bottom: 0.25em;
    }

    .nav-brand {
      width: 60%;
      margin-right: auto;
    }
  }
</style>