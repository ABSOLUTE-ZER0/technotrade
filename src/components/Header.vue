<template>
  <div class="header-div">
    <HeaderTop />
    <HeaderBottom />
  </div>

</template>

<style scoped>
  .br {
    border-bottom: 1px solid rgba(0, 0, 0, 0.075);
    display: block;
    width: 100%;
  }

  .header-div {
    position: sticky;
    top: 0;
    z-index: 30;
    width: 100%;
    background-color: white;
  }
</style>


<script>
  import HeaderTop from "../components/HeaderTop"
  import HeaderBottom from "../components/HeaderBottom"

  export default {
    name: 'Home',
    components: {
      HeaderTop,
      HeaderBottom
    }
  }
</script>