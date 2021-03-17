<template>
  <form class="main-form" action="#" method="post">
          <div class="form">
            <span class="fa fa-user" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" type="text" placeholder="Name" required="">
            </div>
          </div>
          <div class="form">
            <span class="fa fa-mobile" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" type="text" placeholder="Mobile No" required="">
            </div>
          </div>
          
          <div class="form">
            <span class="fa fa-envelope-open-text" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" type="email" placeholder="Email" required="">
            </div>
          </div>
          <div class="form">
            <span class="fa fa-lock" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" type="password" placeholder="Password" required="">
            </div>
          </div>
          <div class="form">
            <span class="fa fa-lock" aria-hidden="true"></span>
            <div class="input-div">
              <input class="input" type="password" placeholder="Confirm Password"
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
</template>

<style scoped>
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