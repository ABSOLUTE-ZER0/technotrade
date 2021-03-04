<template>

    <b-row class="product-div">
      <b-col lg="3">
        <div class="product">
          <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
        </div>
        <b-button class="product-btn">first button</b-button>
        <b-button class="product-btn">second button</b-button>
      </b-col>
      <b-col lg="3">
        <div class="product">
          <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
        </div>
        <b-button class="product-btn">first button</b-button>
        <b-button class="product-btn">second button</b-button>
      </b-col>
      <b-col lg="3">
        <div class="product">
          <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
        </div>
        <b-button class="product-btn">first button</b-button>
        <b-button class="product-btn">second button</b-button>
      </b-col>
      <b-col lg="3">
        <div class="product">
          <img src="https://picsum.photos/1024/480/?image=58" class="add-img" alt="ADD">
        </div>
        <b-button class="product-btn">first button</b-button>
        <b-button class="product-btn">second button</b-button>
      </b-col>
    </b-row>
</template>

<style scoped>
  .product-btn {
    width: 40%;
    margin: 2em .5em;
    font-size: 0.8em;
  }

  .product-div{
    display: flex;
    margin-bottom: 3em;
    margin-top: 1em;
  }
  @media (max-width: 768px) {
  .product-btn {
    width: 40%;
    margin: 1em 0.5em 2em;
    font-size: 0.8em;
  }

  }

</style>