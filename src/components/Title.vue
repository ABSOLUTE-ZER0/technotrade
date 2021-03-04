<template>
      <div class="title-div">
      <h3 class="title">{{title}}</h3>
    </div>
</template>

<style scoped>
  .title {
    text-align: left;
    text-transform: uppercase;
    display: inline-block;
    position: relative;
    background-color: rgb(240, 240, 240);
    padding-right: 0.5em;

  }

  .title-div::before {
    position: absolute;
    content: "";
    width: 98%;
    height: 1px;
    background: rgb(196, 196, 196);
    top: 1em;
    left: 0;
  }

  .title-div {
    position: relative;
    width: 100%;
    text-align: left;
  }

    @media (max-width: 768px) {
  .title {
    font-size: 1.2em;
    font-weight: bold;
  }
    .title-div {
    margin: 1em 0;
  }
    .title-div::before {
    top: 0.6em;
  }
  }


</style>

<script>
export default {
  props: {
    title: String
  }
}
</script>