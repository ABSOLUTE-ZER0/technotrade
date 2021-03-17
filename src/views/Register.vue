<template>
  <b-container fluid class="main">
    <b-row>
      <b-navbar style="width: 100%" class="nav-bar">
        <b-navbar-brand class="brand" href="/">TechoTrade</b-navbar-brand>
        <b-navbar-nav style="margin-left: auto" class="nav-items">
          <b-nav-item href="/login">Login</b-nav-item>
          <b-nav-item href="/register">Register</b-nav-item>
          <b-nav-item href="/about">About Us</b-nav-item>
          <b-nav-item href="/contact">Contact</b-nav-item>
        </b-navbar-nav>
      </b-navbar>
    </b-row>
    <b-row>
      <h1 class="title">Registration form</h1>
    </b-row>
    <b-row>
      <b-col lg="6">
        <h1 class="sub-title">Choose Account Type</h1>
        <AccountType v-on:setType="setType($event)" />
      </b-col>
      <b-col class="form-col" lg="6">
        <SellerRegistration v-if="registerType=='seller'"/>
        <BuyerRegistration v-if="registerType=='buyer'"/>
      </b-col>

    </b-row>
  </b-container>
</template>

<style scoped>
  .main {
    background-image: url("../assets/white.jpg");
    min-height: 100vh;
    background-size: cover;
  }

  .title {
    text-transform: uppercase;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    letter-spacing: 2px;
    text-align: center;
    width: 100%;
    margin-top: 1.5em;
  }

  .sub-title {
    margin: 1.5em 0 1em;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }



  @media (max-width: 768px) {
    .main {
          background-image: url("../assets/white1.jpg");

      font-size: 0.8em;
      background-size: cover;
      height: fit-content;
      padding-bottom: 2em;
      min-height: 100vh;
    }
  }
</style>

<style>
.terms label{
	line-height: 26px;
}

.terms input:focus{
	display: none;
}
</style>


<script>
  import AccountType from "../components/AccountType"
  import SellerRegistration from "../components/SellerRegistration"
  import BuyerRegistration from "../components/BuyerRegistration"

  export default {
    data(){
      return{
        registerType: "buyer"
      }
    },
    components: {
      AccountType,
      SellerRegistration,
      BuyerRegistration
    },
    methods:{
      setType(item){
        this.registerType = item
        console.log(this.registerType);
      }
    }
  }
</script>