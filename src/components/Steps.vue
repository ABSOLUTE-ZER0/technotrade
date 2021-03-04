<template>
  <div class="step-div">
          <h2 class="title">Technotrade procurement solution</h2>

    <div class="step">
      <div class="step-top g1">
        <p>step</p>
        <span>1</span>
      </div>
      <div class="step-main r1">
        <img src="@/assets/t1.png" alt="post your enquiry">
        <div class="step-text">
          <p>post your enquiry</p>
        </div>
      </div>
    </div>
    <div class="step">
      <div class="step-top g2">
        <p>step</p>
        <span>2</span>
      </div>
      <div class="step-main r2">
        <img src="@/assets/t2.png" alt="seller negotiation">
        <div class="step-text">
          <p>seller negotiation</p>
        </div>
      </div>
    </div>
    <div class="step">
      <div class="step-top g3">
        <p>step</p>
        <span>3</span>
      </div>
      <div class="step-main r3">
        <img src="@/assets/t3.png" alt="counter offer">
        <div class="step-text">
          <p>counter<br>offer</p>
        </div>
      </div>
    </div>
    <div class="step">
      <div class="step-top g4">
        <p>step</p>
        <span>4</span>
      </div>
      <div class="step-main r4">
        <img src="@/assets/t4.png" alt="buyer pay-in">
        <div class="step-text">
          <p>buyer<br>pay-in</p>
        </div>
      </div>
    </div>
    <div class="step">
      <div class="step-top g5">
        <p>step</p>
        <span>5</span>
      </div>
      <div class="step-main r5">
        <img src="@/assets/t5.png" alt="inspection of goods">
        <div class="step-text">
          <p>inspection of goods</p>
        </div>
      </div>
    </div>
    <div class="step">
      <div class="step-top g6">
        <p>step</p>
        <span>6</span>
      </div>
      <div class="step-main r6">
        <img src="@/assets/t6.png" alt="delivery of goods">
        <div class="step-text">
          <p>delivery of goods</p>
        </div>
      </div>
    </div>
    <div class="step">
      <div class="step-top g7">
        <p>step</p>
        <span>7</span>
      </div>
      <div class="step-main r7">
        <img src="@/assets/t7.png" alt="payment succesfull">
        <div class="step-text">
          <p>payment successful</p>
        </div>
      </div>
    </div>
  </div>
</template>


<style scoped>

.title{
  font-size: 1.2em;
  font-weight: bold;
}

.step-div h2{
  text-align: left;
  margin-top: 1em;
}
  .step-main::before {
    position: absolute;
    content: "";
    width: 0.9em;
    height: 0.9em;
    bottom: -2.2em;
    right: 1.1em;
    border-radius: 100%;
    z-index: 1;
}

.step-main::after {
    position: absolute;
    content: "";
    width: 0;
    height: 0;
    border-top: 1.7em solid white;
    border-right: 1.6em solid transparent;
    bottom: -1.7em;
    right: 0;
}

  .step-top::after {
    position: absolute;
    content: "";
    width: 0;
    height: 0;
    border-left: 1em solid transparent;
    left: 0;
    top: 2.5em;
}

  .step-top span {
    position: absolute;
    background: white;
    top: 0.25em;
    right: 0.5em;
    width: 1.5em;
    height: 1.5em;
    border-radius: 50%;
    font-size: 1.2em;
    font-weight: 600;
    display: flex;
    align-items: center;
    justify-content: center;
    color: gray;
}

  .step-top p {
    position: relative;
    font-size: 0.9em;
    color: white;
    text-transform: uppercase;
    font-weight: 600;
    margin-top: 0.2em;
    letter-spacing: 0.25em;
}

  .step-text {
    width: 100%;
    float: left;
    position: relative;
    padding-top: 0.5em;
}

  .step-main {
    width: 100%;
    height: 100%;
    position: relative;
    float: left;
    background: white;
    border-radius: 0 0 0 20%;
    padding: 2.2em;
    padding-left: 1.5em;
    padding-right: 1.5em;
}


  .step-top{
    position: absolute;
    width: 80%;
    height: 2.5em;
    background: red;
    left: 0;
    z-index: 1;
    border-radius: 0 20px 20px 0;
    top: 0;
    padding: 0.5em;
    padding-left: 1em;
}

  .step {
    width: 14%;
    min-width: 13em;
    float: left;
    height: 11em;
    position: relative;
    padding: 1em;
    margin-top: 2em;
}

  .step-div {
    width: 100%;
    position: relative;
    float: left;
    padding-bottom: 1em !important;
    border-bottom: 5px solid #fff;
    background-color: rgb(206, 154, 255);
    padding: 0 10%;
}


  .g1 {
    background-image: var(--g1-gredient) !important;
  }

  .g2 {
    background-image: var(--g2-gredient) !important;
  }
  .g3 {
    background-image: var(--g3-gredient) !important;
  }
  .g4 {
    background-image: var(--g4-gredient) !important;
  }
  .g5 {
    background-image: var(--g1-gredient) !important;
  }
  .g6 {
    background-image: var(--g3-gredient) !important;
  }
  .g7 {
    background-image: var(--g4-gredient) !important;
  }

  
  .g1::after{
    border-top: var(--g1-after);

  }
  
  .g2::after{
    border-top: var(--g2-after);

  }
  
  .g3::after{
    border-top: var(--g3-after);

  }
  
  .g4::after{
    border-top: var(--g4-after);

  }
  .g5::after{
    border-top: var(--g1-after);

  }
  .g6::after{
    border-top: var(--g3-after);

  }
  .g7::after{
    border-top: var(--g4-after);

  }

  .r1::before {
    background-image: var(--g1-gredient);
}
  .r2::before {
    background-image: var(--g2-gredient);
}
  .r3::before {
    background-image: var(--g3-gredient);
}
  .r4::before {
    background-image: var(--g4-gredient);
}
  .r5::before {
    background-image: var(--g1-gredient);
}
  .r6::before {
    background-image: var(--g3-gredient);
}
  .r7::before {
    background-image: var(--g4-gredient);
}


  @media (max-width: 768px) {
  .step {
    width: 50%;
    min-width: 10em;
}

  .step-div {
    padding: 0 1.3em;
}

  .step-main::before {
    display: none;

}

.step-main::after {
    display: none;
}


  }



</style>

<style>
  :root{
    --g1-after: 16px solid #4672ce;
    --g2-after: 16px solid #c56b6b;
    --g3-after: 16px solid #dc8e47;
    --g4-after: 16px solid #3fb995;
    --g1-gredient: linear-gradient(to right, #32a5f8, #2c92fb, #487cf8, #6b61ed, #8b3bda);
    --g2-gredient: linear-gradient(to right, #f48071, #f57277, #f3657f, #ef5889, #e74d96);
    --g3-gredient: linear-gradient(to right, #ffb772, #ffac6e, #ffa06b, #ff946a, #ff886b);
    --g4-gredient: linear-gradient(to right, #06df98, #00d2a5, #00c4ad, #00b5af, #01a6ac);
  }
</style>