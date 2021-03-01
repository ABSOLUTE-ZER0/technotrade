<template>
  <div class="header-top">
      <b-navbar toggleable="lg">
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse style="text-align: center;width:100%" id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/msg.png"> info@technotrade.com
            </b-nav-item>
            <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/call.png"> +91 99999 99999
            </b-nav-item>
          </b-navbar-nav>

          <!-- Right aligned nav items -->
          <b-navbar-nav style="text-align: center" class="ml-auto">
            <b-nav-item class="nav-item" href="#"><img class="navtop-img" src="@/assets/mobile.png"> Download App
            </b-nav-item>
            <b-nav-item class="nav-item" href="#"> Sell on Technotrade</b-nav-item>
            <b-nav-item class="nav-item" href="#"> Careers</b-nav-item>
            <b-nav-item-dropdown class="nav-item" text="Lang" right>
              <b-dropdown-item href="#">EN</b-dropdown-item>
              <b-dropdown-item href="#">AR</b-dropdown-item>
              <b-dropdown-item href="#">FR</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-button class="signin-btn" variant="outline-warning">Sign In</b-button>

          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
</template>

<style scoped>
  .nav-item {
    margin: 0 1em;

  }

  .header-top {
    background-color: white;
    font-size: 0.9em;
      padding: 0 10%;

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
</style>