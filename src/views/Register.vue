<template>
  <b-container fluid class="main">
    <b-row>
      <b-navbar style="width: 100%" class="nav-bar">
        <b-navbar-brand class="brand" href="/">TechnoTrade</b-navbar-brand>
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
        <AccountType />
      </b-col>
      <b-col class="form-col" lg="6">
        <form class="main-form" action="#" method="post">
          <div class="form">
            <span class="fa fa-user" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" name="text1" id="text1" type="text" value="" placeholder="Name" required="">
            </div>
          </div>
          <div class="form">
            <span class="fa fa-mobile" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" name="text1" id="text1" type="text" value="" placeholder="Mobile No" required="">
            </div>
          </div>
          <div class="form">
            <span class="fa fa-envelope-open-text" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" name="text1" id="text1" type="email" value="" placeholder="Email" required="">
            </div>
          </div>
          <div class="form">
            <span class="fa fa-lock" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" name="text1" id="text1" type="password" value="" placeholder="Password" required="">
            </div>
          </div>
          <div class="form">
            <span class="fa fa-lock" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" name="text1" id="text1" type="password" value="" placeholder="Confirm Password"
                required="">
            </div>
          </div>
          <b-form-checkbox class="terms" id="checkbox-1" name="checkbox-1" value="accepted">
            I accept the terms and conditions
          </b-form-checkbox>
          <div style="width:100%;text-align: left;">
            <button type="submit" class="btn">Get Started</button>
          </div>
        </form>

      </b-col>

    </b-row>
  </b-container>
</template>

<style scoped>
  .main {
    background-image: url("../assets/white.jpg");
    height: 100vh;
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

  .main-form {
    margin-left: 20%;
    margin-top: 5em;
  }

  .form {
    display: flex;
    margin: 1em 0;
    background-color: rgba(186, 149, 255, 0.2);
    border-radius: 2em;
    width: 70%;
  }

  .form span {
    flex: 1;
    line-height: 3em;
    margin-top: 0.1em;
    text-align: right;
  }

  .input-div {
    flex: 4 50%;
  }

  .input {
    padding: 1em;
    background-color: transparent;
    border: 0;
    width: 100%;
  }

  .input:focus {
    outline: 0;
  }

  .terms {
    text-align: left;
    margin-bottom: 1em;
  }

  .btn {
    background-color: rgb(146, 87, 255);
    width: 70%;
    color: white;
    border-radius: 2em;
    font-size: 1.2em;
    letter-spacing: 2px;
    margin-left: 0;
  }

  @media (max-width: 768px) {
    .main {
      font-size: 0.8em;
      background-size: cover;
      height: fit-content;
      padding-bottom: 2em;
      min-height: 100vh;
    }

    .brand{
      font-size: 1em;
      font-weight: bold;
      margin-right: 0;
    }

    .title {
      margin-top: 1em;
      font-size: 1.8em;
    }

    .sub-title {
      font-size: 1.3em;
    }

    .main-form {
      margin-top: 2em;
      margin-left: 10%;
    }

    .form {
      width: 90%;
    }

    .btn {
      width: 50%;
      margin-left: 40%;
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

  export default {
    components: {
      AccountType
    }
  }
</script>