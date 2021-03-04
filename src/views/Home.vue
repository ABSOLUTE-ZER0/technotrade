<template>
  <div>
    <Header />
    <b-container fluid class="main-container">
      <b-row class="carousel-row">
        <b-col lg="3" class="col1 d-none d-lg-block">
          <SelectProduct />
          <Qr />
        </b-col>
        <b-col class="col1 carousel-div comp" lg="6">
          <Carousel />
        </b-col>
        <b-col class="col1" style="margin-bottom: 2em" lg="3">
          <Add />
        </b-col>
      </b-row>

      <b-row class="caption-row">
        <b-col class="col1">
          <div class="caption">
            <p class="caption-text">BUY OR SELL GLOBALLY WITHOUT A PHONE CALL OR AN EMAIL</p>
          </div>
        </b-col>
      </b-row>

      <b-row style="margin: 2em 0">
        
        <b-col class="col1" lg="6">
          <LiveCount />
        </b-col>

        <b-col class="col1 test" lg="4">
          <div style="height: 100%;" class="comp">
            <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
          </div>
        </b-col>

        <b-col class="col1 test" lg="2">
          <div style="height: 100%;" class="comp">
            <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
          </div>
        </b-col>
      </b-row>

      <b-row class="">
        <b-col class="col1">
          <About />
        </b-col>
      </b-row>


      <b-row style="margin: 1em 0">
        <b-col class="col1" lg="4">
          <Why />


        </b-col>

        <b-col class="col1" lg="8">
          <Title title="HOW WE HELPS SUPPLIERS" />
          <b-row class="how-help">
            <b-col lg="3" class="help">
              <img src="https://picsum.photos/1024/480/?image=58" class="help-img" alt="ADD">
            </b-col>
            <b-col lg="3" class="help">
              <img src="https://picsum.photos/1024/480/?image=58" class="help-img" alt="ADD">
            </b-col>
            <b-col lg="3" class="help">
              <img src="https://picsum.photos/1024/480/?image=58" class="help-img" alt="ADD">
            </b-col>
            <b-col lg="3" class="help">
              <img src="https://picsum.photos/1024/480/?image=58" class="help-img" alt="ADD">
            </b-col>
          </b-row>
        </b-col>

      </b-row>

                <Title title="Technotrade videos" />

      <b-row class="video-row">
        <b-col class="col1" lg="6">
          <div class="video">
            <h3 class="video-title">Buyer Process</h3>
            <b-embed type="iframe" aspect="16by9" src="https://www.youtube.com/embed/uT0VzQBPe10" allowfullscreen>
            </b-embed>
          </div>
        </b-col>
        <b-col class="col1" lg="6">
          <div class="video">
            <h3 class="video-title">Sellers Process</h3>
            <b-embed type="iframe" aspect="16by9" src="https://www.youtube.com/embed/uT0VzQBPe10" allowfullscreen>
            </b-embed>
          </div>
        </b-col>
      </b-row>
      <b-row>

                        <Title title="Technotrade products" />
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




  .carousel-div.comp {
    padding: 0;
  }

  .help {
    height: 100%;
    margin: 1em 0;

  }

  .help-img {
    width: 100%;
    height: 200%;
  }

  .caption-row {
    margin: 1.5em 0;
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

  @media (max-width: 768px) {
    .col1 {
      padding: 0;
    }

    .caption {
      background-color: rgb(255, 81, 0);
      border-radius: 0.5em;
      color: white;
      font-size: 1.1em;
      font-weight: 600;
      padding: 0.5em 0;
    }

    .caption-text {
      text-align: center;
      width: 100%;
      margin: 0;
      text-shadow: 4px 4px 4px rgb(78 78 80 / 33%);
    }

    .caption-row {
      margin: 0 -15px;
    }

    .test{
      margin: 1em -15px;
    }

  .video-title{
    font-size: 1.1em;
    text-align: left;
    margin-top: 1.1em;
  }


  }
</style>

<style>
  .add-img {
    width: 100%;
    height: 100%;
    background-color: #343434;
  }

  .comp {
    background-color: white;
    margin: 1em 0em;
    border-radius: 0.5em;

  }


</style>

<script>
  import Header from "../components/Header"
  import Steps from "../components/Steps"
  import Products from "../components/Products"
  import SelectProduct from "../components/SelectProduct"
  import Qr from "../components/QrCode"
  import Carousel from "../components/Carousel"
  import Add from "../components/Add"
  import LiveCount from "../components/LiveCount"
  import About from "../components/About"
  import Why from "../components/Why"
  import Title from "../components/Title"


  export default {
    name: 'Home',
    components: {
      Header,
      Steps,
      Products,
      SelectProduct,
      Qr,
      Carousel,
      Add,
      LiveCount,
      About,
      Why,
      Title
    }
  }
</script>