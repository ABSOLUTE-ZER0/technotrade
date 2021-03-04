<template>
  <div class="selectproduct-div comp">
    <h3 class="product-title">Select Product</h3>
    <b-dropdown menu-class="w-100" id="dropdown-1" text="Product Segment" class="product-dropdown m-md-2">
      <b-dropdown-item>First</b-dropdown-item>
      <b-dropdown-item>Second</b-dropdown-item>
      <b-dropdown-item>Third</b-dropdown-item>
    </b-dropdown>
    <b-dropdown menu-class="w-100" id="dropdown-2" text="Commodities" class="product-dropdown m-md-2">
      <b-dropdown-item>First</b-dropdown-item>
      <b-dropdown-item>Second</b-dropdown-item>
      <b-dropdown-item>Third</b-dropdown-item>
    </b-dropdown>
    <b-dropdown menu-class="w-100" id="dropdown-3" text="Product" class="product-dropdown m-md-2">
      <b-dropdown-item>First</b-dropdown-item>
      <b-dropdown-item>Second</b-dropdown-item>
      <b-dropdown-item>Third</b-dropdown-item>
    </b-dropdown>
    <b-button class="product-submit">Submit</b-button>
  </div>
</template>

<style scoped>
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
</style>

<style>
  #dropdown-1__BV_toggle_,
  #dropdown-2__BV_toggle_,
  #dropdown-3__BV_toggle_ {
    background-color: white;
    color: black;
  }
</style>