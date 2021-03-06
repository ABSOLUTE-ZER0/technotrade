<template>
  <div class="header-top">
    <div class="header">
      <b-navbar>
        <b-navbar-nav class="d-none d-lg-flex">
          <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/msg.png"> info@technotrade.com
          </b-nav-item>
          <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/call.png"> +91 99999 99999
          </b-nav-item>
        </b-navbar-nav>

        <b-navbar-nav style="text-align: center" class="d-none d-lg-flex right">
          <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/mobile.png"> Download App
          </b-nav-item>
          <b-nav-item class="nav-item" href="#"> Sell on Technotrade</b-nav-item>
          <b-nav-item class="nav-item" href="#"> Careers</b-nav-item>
          <b-nav-item-dropdown class="nav-item" text="Lang" right>
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">AR</b-dropdown-item>
            <b-dropdown-item href="#">FR</b-dropdown-item>
          </b-nav-item-dropdown>

        </b-navbar-nav>

        <b-navbar-nav class="d-lg-none">
          <p>Choose language: </p>
          <b-nav-item class="nav-item" href="#"> EN</b-nav-item> |
          <b-nav-item class="nav-item" href="#"> AR</b-nav-item> |
          <b-nav-item class="nav-item" href="#"> FR</b-nav-item> |
        </b-navbar-nav>
      </b-navbar>
    </div>
    <div class="button">
      <b-button-group>
      <b-dropdown variant="outline-warning" class="signin-btn" right text="Sign In">
      <b-dropdown-item href="/login">Login</b-dropdown-item>
      <b-dropdown-item href="/register">Register</b-dropdown-item>
    </b-dropdown>
      </b-button-group>
    </div>


  </div>
</template>

<style scoped>
  .nav-item {
    margin: 0 1em;
  }

  .header {
    width: 95%;
    display: inline-block;
  }

  .button {
    display: inline-block;
    width: 5%;
  }

  .header-top {
    background-color: white;
    font-size: 0.9em;
    margin: 0 10%;
  }

  .right {
    margin-left: auto;
  }

  .navtop-img {
    width: 1em;
    margin-bottom: 0.25em;
  }

  .signin-btn {
    font-weight: bold;
    color: orangered;
    font-size: 1em;
  }

  @media (max-width: 1000px) and (min-width: 768px) {}

  @media (max-width: 768px) {
    .nav-item {
      margin: -0.5em 0;
    }
  .header {
    width: 75%;
    float: left;
  }

    .header-top {
    margin: 0;
    width: 100%;
  }
  .button {
    width: 25%;
  }




  }
</style>