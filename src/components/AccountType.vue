<template>
<div>
  <div class="type">
    <input checked @click="accountType='buyer'" type="radio" name="user" id="cb1" value="buyer" />
    <label class="lab1" for="cb1"><img src="../assets/buyer.jpg" /></label>
    <input @click="accountType='seller'" type="radio" name="user" id="cb2" value="seller" />
    <label for="cb2"><img src="../assets/seller.jpg" /></label>
  </div>
  <div>
    <p class="sub">Hello <strong>{{accountType}}  </strong> </p>
    <p class="sub">Fill out the form to get started</p>
  </div>
</div>


</template>

<style scoped>

  .type{
    display: flex;
    width: 100%;
    align-items: center;
    margin-bottom: 2em;
  }
  input {
    display: none;
  }

  .lab1{
    margin-left: 20%;
  }

  label {
    display: block;
    position: relative;
    cursor: pointer;
    width: 25%;
    margin-left: 10%;
  }

  label::after {
    background-color: white;
    color: white;
    content: " ";
    display: block;
    border-radius: 50%;
    position: absolute;
    width: 30px;
    height: 30px;
    bottom: 0;
    right: 0;
    text-align: center;
    line-height: 32px;
    transition-duration: 0.4s;
    transform: scale(0);
  }

  label img {
    width: 100%;
    transition-duration: 0.2s;
    transform-origin: 30% 30%;
  }

  :checked+label::after {
    content: "✓";
    background-color: rgb(110, 125, 255);
    transform: scale(1);
    position: absolute;
    z-index: 2;
    bottom: 0;
    right: 0;
  }

  :checked+label img {
    transform: scale(0.95);
  }

  .sub{
    color: grey;
    font-family: cursive;
    font-size: 1.1em;
  }

    @media (max-width: 768px){
  label::after{
        width: 22px;
    height: 22px;
    line-height: 24px;
    vertical-align: middle;
  }
    }
</style>

<script>
export default {
  data(){
    return{
      accountType: "buyer"
    }
  }
}
</script>