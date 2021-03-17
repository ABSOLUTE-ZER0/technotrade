<template>
  <div>
    <div class="title-div">
      <h1 class="title">Vendor details</h1>
    </div>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Name</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Membership Type</h1>
      </b-col>
      <b-col lg="5">
        <b-form-select v-model="selectedMembership" :options="options"></b-form-select>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Company Details</h1>
      </b-col>
      <b-col lg="5">
        <b-form-textarea rows="3" no-resize></b-form-textarea>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Authorized Person</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Legal Documents</h1>
      </b-col>
      <b-col lg="5">
        <b-form-file accept=".pdf" v-model="file1" :state="Boolean(file1)" placeholder="Choose a file or drop it here..."
          drop-placeholder="Drop file here..."></b-form-file>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Bank Details</h1>
      </b-col>
      <b-col lg="5">
        <b-form-textarea rows="2" no-resize></b-form-textarea>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Selling Location</h1>
      </b-col>
      <b-col lg="5">
        <b-form-textarea rows="3" no-resize></b-form-textarea>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Type</h1>
      </b-col>
      <b-col lg="5">
        <b-form-radio-group class="type" id="radio-slots" v-model="selectedTypeRadio" :options="optionsRadio"
          :aria-describedby="ariaDescribedby" name="radio-options-slots"> </b-form-radio-group>
      </b-col>
    </b-row>
    <div class="save-div">
    <b-button class="save-btn" variant="success">Save</b-button>

    </div>
  </div>
</template>


<style scoped>
  .title-div {
    width: 100%;
    background-color: rgb(202, 202, 202);
    text-align: left;
    margin-top: 20px;
    padding: 5px;
    margin-bottom: 20px;
  }

  .detail-row {
    margin-bottom: 10px;
  }

  .title {
    font-size: 1.3em;
    font-weight: bold;
    margin-left: 5px;
    text-transform: uppercase;
  }

  .sub-title {
    width: 100%;
    text-align: left;
    font-size: 1.2em;
    margin-top: 10px;
  }

  .type{
    margin-top: 10px;
  }

  .save-div{
    text-align: left;
  }

  .save-btn{
    width: 12%;
    margin-top: 10px;
    margin-left: 45%;
  }
</style>






<script>
  export default {
    data() {
      return {
        selectedMembership: null,
        selectedTypeRadio: "",
        options: [{
            value: null,
            text: ' -- Please select a Membership Type -- ',
            disabled: true
          },
          {
            value: 'Quarter',
            text: 'Quarter Subscription'
          },
          {
            value: 'Half',
            text: 'Half Yearly Subscription'
          },
          {
            value: 'Yearly',
            text: 'Yearly Subscription'
          }
        ],
        optionsRadio: [{
            text: 'Bulk',
            value: 'Bulk'
          },
          {
            text: 'Retail',
            value: 'Retail'
          }
        ]
      }
    }
  }
</script>


<b-form-file v-model="file1" :state="Boolean(file1)" placeholder="Choose a file or drop it here..."
  drop-placeholder="Drop file here..."></b-form-file>