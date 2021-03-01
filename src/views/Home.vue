<template>

  <div>
    <Header />
    <b-container fluid class="main-container">
      <b-row class="carousel-row">
        <b-col lg="3" class="">
          <div class="selectproduct-div comp">
            <h3 class="product-title">Select Product</h3>
            <b-dropdown menu-class="w-100" id="dropdown-1" text="Product Segment" class="product-dropdown m-md-2">
              <b-dropdown-item>First</b-dropdown-item>
              <b-dropdown-item>Second</b-dropdown-item>
              <b-dropdown-item>Third</b-dropdown-item>
            </b-dropdown>
            <b-dropdown menu-class="w-100" id="dropdown-1" text="Commodities" class="product-dropdown m-md-2">
              <b-dropdown-item>First</b-dropdown-item>
              <b-dropdown-item>Second</b-dropdown-item>
              <b-dropdown-item>Third</b-dropdown-item>
            </b-dropdown>
            <b-dropdown menu-class="w-100" id="dropdown-1" text="Product" class="product-dropdown m-md-2">
              <b-dropdown-item>First</b-dropdown-item>
              <b-dropdown-item>Second</b-dropdown-item>
              <b-dropdown-item>Third</b-dropdown-item>
            </b-dropdown>
            <b-button class="product-submit">Submit</b-button>
          </div>
          <div class="comp">
            <b-row>
              <b-col md="auto">
                <img class="qr" src="@/assets/qr.png">
              </b-col>
              <b-col md="7">
                <div class="qr_text">
                  <h3>Download Buyer App</h3>
                  <p>Scan to download</p>
                </div>
              </b-col>
            </b-row>

          </div>
        </b-col>
        <b-col class="carousel-div comp" lg="6">
          <b-carousel id="carousel-1" v-model="slide" :interval="4000" controls indicators background="#ababab"
            img-width="1024" img-height="480" style="text-shadow: 1px 1px 2px #333;">

            <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=52"></b-carousel-slide>

            <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=54"></b-carousel-slide>

            <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=58"></b-carousel-slide>

            <b-carousel-slide>
              <template #img>
                <img class="d-block img-fluid w-100" width="1024" height="480"
                  src="https://picsum.photos/1024/480/?image=55" alt="image slot">
              </template>
            </b-carousel-slide>

          </b-carousel>
        </b-col>
        <b-col class="comp" lg="3">
          <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
        </b-col>
      </b-row>

      <b-row style="margin: 1.5em 0" class="">
        <b-col>
          <div class="caption">
            <p class="caption-text">BUY OR SELL GLOBALLY WITHOUT A PHONE CALL OR AN EMAIL</p>

          </div>

        </b-col>
      </b-row>

      <b-row style="margin: 2em 0">
        <b-col lg="6">
          <div class="live-count comp">

            <div class="live-common">
              <div class="live-img">
                <img src="@/assets/live.png" alt="live">
              </div>
              <div class="live-text">
                <h3 class="live-text">Registered<br>Agri Buyers</h3>
              </div>
            </div>

            <div class="live-common">
              <div class="live-img">
                <img src="@/assets/nego.png" alt="nego">
              </div>
              <div class="live-text">
                <h3 class="live-text">Registered<br>Construction Buyers</h3>
              </div>
            </div>

            <div class="live-common">
              <div class="live-img">
                <img src="@/assets/order.png" alt="order">
              </div>
              <div>
                <h3 class="live-text">Registered<br>Sellers</h3>
              </div>
            </div>

          </div>
        </b-col>
        <b-col lg="4">
          <div style="height: 100%;" class="comp">
            <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
          </div>
        </b-col>

        <b-col lg="2">
          <div style="height: 100%;" class="comp">
            <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
          </div>
        </b-col>

      </b-row>

      <b-row style="margin: 1em 0">
        <b-col>
          <div class="about comp">
            <h3 class="about-heading">What Is Technotrade</h3>
            <p class="about-text">Some random Text.</p>
            <b-button href="#" variant="info">Read More</b-button>
          </div>
        </b-col>

      </b-row>


      <b-row style="margin: 1em 0">
        <b-col lg="4">
          <h3>HOW WE HELPS SUPPLIERS</h3>

          <div class="trade-under comp">
            <div class="why-icon">
              <img src="@/assets/w4.png" alt="Trade Across The World">
              <div class="why-text">
                <p>Trade Across The World</p>
              </div>
            </div>
            <div class="why-icon">
              <img src="@/assets/w3.png" alt="Completely Transparent">
              <div class="why-text">
                <p>Completely Transparent</p>
              </div>
            </div>
            <div class="why-icon">
              <img src="@/assets/w2.png" alt="Modelled Around Bussiness">
              <div class="why-text">
                <p>Modelled Around Bussiness</p>
              </div>
            </div>
            <div class="why-icon">
              <img src="@/assets/w1.png" alt="Cost Effective">
              <div class="why-text">
                <p>Cost Effective</p>
              </div>
            </div>

          </div>
        </b-col>

        <b-col lg="8">
          <h3>HOW WE HELPS SUPPLIERS</h3>
          <div class="how-help">
            <div class="help comp">
              <img src="https://picsum.photos/1024/480/?image=58" class="help-img" alt="ADD">
            </div>
            <div class="help comp">
              <img src="https://picsum.photos/1024/480/?image=58" class="help-img" alt="ADD">
            </div>
            <div class="help comp">
              <img src="https://picsum.photos/1024/480/?image=58" class="help-img" alt="ADD">
            </div>
            <div class="help comp">
              <img src="https://picsum.photos/1024/480/?image=58" class="help-img" alt="ADD">
            </div>
          </div>
        </b-col>

      </b-row>
      <h2>Technotrade videos</h2>

      <b-row>
        <b-col lg="6">
          <div class="video">
            <p>Buyer Process</p>
            <b-embed type="iframe" aspect="16by9" src="https://www.youtube.com/embed/uT0VzQBPe10" allowfullscreen>
            </b-embed>
          </div>
        </b-col>
        <b-col lg="6">
          <div class="video">
            <p>Sellers Process</p>
            <b-embed type="iframe" aspect="16by9" src="https://www.youtube.com/embed/uT0VzQBPe10" allowfullscreen>
            </b-embed>
          </div>
        </b-col>
      </b-row>
      <b-row>
      <h2 style="margin-top: 2em">Technotrade products</h2>
      <Products />
      </b-row>
    </b-container>
          <Steps />
  </div>

</template>


<style scoped>
  .main-container {
    padding: 0 10%;
  }

  .how-help {
    display: flex;

  }

  .help {
    height: 100%;
  }

  .help-img{
    width: 100%;
    height: 200%;
  }

  .trade-under {
    margin: 1em;
    display: block;
  }

  .why-icon {
    min-width: 50%;
    padding: 1em;
    display: inline-block;
    border: 1px solid #e6e6e6;

  }


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
    padding-left: 30px;
    padding-right: 30px;
  }

  .about {
    text-align: center;
    width: 100%;
    position: relative;
    background-color: #fff;
    border: 1px solid #e6e6e6;
    padding: 1em 0;
  }

  .live-common {
    width: 33.33%;
    display: flex;
    padding: 1em;
    border: 1px solid #e6e6e6;
  }

  .live-text {
    font-size: 0.9em;
    color: grey;
    text-align: left;
    margin: 0.1em;
  }

  .live-count {
    display: flex;
    height: 100%;

  }

  .caption {
    background-color: rgb(255, 81, 0);
    border-radius: 0.5em;
    color: white;
    font-size: 1.5em;
  }

  .caption-text {
    text-align: center;
    width: 100%;
    margin: 0.5em;
  }



  .product-title {
    margin-top: 1em;
    font-weight: bold;
  }

  .product-submit {
    margin: 0.5em;
    margin-bottom: 2em;
  }

  .selectproduct-div {
    display: flex;
    flex-direction: column;
  }

  .qr {
    width: 7em;
  }

  .qr_text {
    margin-left: -1em;
    text-align: left;
    margin-top: 0.5em;
  }

  .carousel-row {
    margin-top: 1em;
  }

  .comp {
    background-color: white;
    margin: 1em 0em;
    border-radius: 0.5em;

  }

  .carousel-div {
    margin: 1em 0;
  }


</style>

<style>
  #dropdown-1__BV_toggle_ {
    background-color: white;
    color: black;
  }

  .add-img {
    width: 100%;
    height: 100%;
    background-color: #343434;
  }

</style>

<script>
  import Header from "../components/Header"
  import Steps from "../components/Steps"
  import Products from "../components/Products"
  export default {
    name: 'Home',
    components: {
      Header,
      Steps,
      Products
    }
  }
</script>