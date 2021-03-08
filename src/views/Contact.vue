<template>
  <div>
    <Header />
    <div class="img">
    </div>
    <b-container>
      <b-col class="main-col">
        <row>
          <h4 class="title">Get In Touch</h4>
          <p class="desc">Do you have any Queries or Have sales/advertising queries or looking for any other
            informationFill out the form below and we will get back to you at the earliest.</p>
        </row>
      </b-col>
      <b-row style="margin-bottom: 2em;">
        <b-col class="input-col" lg="6">
          <div class="input-div">
            <b-input class="input" type="text" placeholder="Full Name" required=""></b-input>
          </div>
          <div class="input-div">
            <b-input class="input" type="text" placeholder="Email ID" required=""></b-input>
          </div>
          <div class="input-div">
            <b-input class="input" type="text" placeholder="Mobile Number" required=""></b-input>
          </div>
          <div class="input-div">
            <b-input class="input" type="text" placeholder="Country" required=""></b-input>
          </div>
          <div class="input-div">
            <b-form-textarea no-resize class="input" type="text-area" placeholder="Message" required="">
            </b-form-textarea>
          </div>
          <div>
            <b-button class="submit-btn">Submit</b-button>
          </div>

        </b-col>
        <b-col lg="6">
          <div>
            <div>
              <div class="title1"> <i class="fa fa-envelope" aria-hidden="true"></i> Connect with Us</div>
              <p>For Support, information or Queries email us at <br><a>info@technotrade.org</a></p>
            </div>
            <div>
              <div class="title1"><i class="fa fa-phone-square" aria-hidden="true"></i> Please call Us at
              </div>
              <p>+91 7354213542, +91 3521402356</p>
            </div>
            <div>
              <div>GLOBAL HEADQUARTER</div>
              <div class="title2">TECHNOTRADE</div>
              <p>Wertdfyujgkmhgnfvdcx</p>
            </div>
            <div>
              <div class="title2">zegrthyjkiyugtrdfsd</div>
              <div>wzrthfyguijkljhg</div>
              <p>sdfghfghfdfg</p>
            </div>
          </div>

        </b-col>
      </b-row>

    </b-container>
  </div>

</template>

<style scoped>
  .main-col {
    text-align: left;
    line-height: 2em;
  }

  .img {
    width: 100%;
    height: 28em;
    background-image: url("../assets/contact.jpg");
    background-size: cover;
    background-position: center;
    margin-bottom: 4em;
  }

  .title {
    font-size: 2em;
    color: black;
    text-shadow: 1px 1px grey;
    margin: 2em 0 0.5em;
    width: fit-content;
  }

  .desc {
    font-weight: bold;
    color: rgb(46, 46, 46);
  }

  .input {
    margin: 2em 0;
  }

  .input-col {
    border: 2px solid orangered;
    padding: 1em 3em 1em;
    border-radius: 1em;
  }


  .submit-btn {
    background-color: orangered;
    border: 0;
    width: 30%;
  }

  .title1 {
    font-size: 1.3em;
    color: black;
    font-weight: bold;
    margin: 2em 0 0.5em;
  }

  .title2 {
    font-size: 1.3em;
    color: orange;
    margin: 2em 0 0.5em;
  }

  @media (max-width: 768px) {
    .main-col {
      font-size: 0.8em;
      text-align: center;
    }
    .desc {
    width: 100%;
  }

    .title {
    font-size: 1.5em;
    margin: 1em 0 0.5em;
    width: 100%;
  }

    .input-col {
    border: 2px solid orangered;
    padding: 1em 2em;
    border-radius: 1em;
    margin: 1em;
  }


    .img {
      height: 8em;
      margin-bottom: 0em;
    }

  }
</style>

<script>
  import Header from "../components/Header"

  export default {
    components: {
      Header
    }
  }
</script>