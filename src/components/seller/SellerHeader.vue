<template>
  <div class="header-bottom">
    <b-navbar class="nav-bar" toggleable="lg">
      <b-navbar-brand class="nav-brand" href="/seller">
        TechoTrade.org: Seller Control Panel
      </b-navbar-brand>

      <b-navbar-toggle class="toggle-btn" target="nav-collapse"></b-navbar-toggle>

      <b-collapse style="text-align: center;width:100%" id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item class="nav-item" href="/"> Home</b-nav-item>
          <b-nav-item class="nav-item" href="/about">About Us
          </b-nav-item>
          <b-nav-item class="nav-item" href="/contact"> Contact Us</b-nav-item>
          <b-nav-item class="nav-item" href="#"> UserName</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<style scoped>
  .nav-item {
    margin: 0 1em;
    font-size: 1em;
    font-weight: bold;
  }

  .nav-bar{
    padding: 0.5em 0;
  }

  .header-bottom {
    background-color: rgb(0, 204, 255);
    font-size: 0.9em;
    padding: 0 10%;
    margin-bottom: 0.5em;
  }

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
      margin: 0;
      padding: 0;
    }

    .nav-brand {
      font-size: 1em;
      margin-top: 1em;
      padding-bottom: 1em;
      width: fit-content;
    }
  }
</style>