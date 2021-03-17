<template>
  <div>
    <div class="title-div">
      <h1 class="title">Company Details</h1>
    </div>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Vendor Short Name</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Company Name</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Company Type</h1>
      </b-col>
      <b-col lg="5">
        <b-form-select v-model="companyType" :options="optionsCompany"></b-form-select>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Company GST No.</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Company Pan No.</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Incorporation Date	</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Time Zone</h1>
      </b-col>
      <b-col lg="5">
        <b-form-select v-model="companyType" :options="optionsTimeZone"></b-form-select>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Country</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">State/Province</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">City</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Area</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Address</h1>
      </b-col>
      <b-col lg="5">
        <b-form-textarea rows="3" no-resize></b-form-textarea>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Zip/Postal Code</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Group</h1>
      </b-col>
      <b-col lg="5">
        <b-form-select v-model="companyType" :options="optionsGroup"></b-form-select>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Retail Min Quantity</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Retail Max Quantity</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Bulk Min Quantity</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Bulk Max Quantity</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Priority</h1>
      </b-col>
      <b-col lg="5">
        <b-form-input></b-form-input>
      </b-col>
    </b-row>
    <b-row class="detail-row">
      <b-col lg="2">
        <h1 class="sub-title">Bidding</h1>
      </b-col>
      <b-col lg="5">
<b-form-radio-group class="type" id="radio-slots" v-model="selectedTypeRadio" :options="optionsRadio"
          :aria-describedby="ariaDescribedby" name="radio-options-slots"> </b-form-radio-group>      </b-col>
    </b-row>

    <div class="save-div">
    <b-button class="submit-btn" variant="success">Submit</b-button>
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

  .save-div{
    text-align: left;
  }

  .type{
    margin-top: 10px;
  }

  .submit-btn{
    width: 12%;
    margin-top: 10px;
    margin-left: 45%;
    margin-bottom: 50px;
  }
</style>






<script>
  export default {
    data() {
      return {
        companyType: "",
        file1: null,
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
            text: 'Yes',
            value: 'Yes'
          },
          {
            text: 'No',
            value: 'No'
          }
        ]
      }
    }
  }
</script>


<b-form-file v-model="file1" :state="Boolean(file1)" placeholder="Choose a file or drop it here..."
  drop-placeholder="Drop file here..."></b-form-file>