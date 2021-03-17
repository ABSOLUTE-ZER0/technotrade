<template>
  <div>
    <div class="title-div">
      <h1 class="title">Membership Details</h1>
    </div>
    <div class="table-div">
      <b-table table-variant="info" striped hover head-variant="dark" :items="items"></b-table>
    </div>
    <b-row style="margin-top: 40px">
      <b-col lg="6" class="offer-div">
        <h1 class="title">Offer</h1>
        <span class="offer">✔ The Cost of Membership includes Service Tax @ 15%. <br>
          ✔ Any Convenience Fee, if applicable shall be charged extra.<br>
          ✔ The rates for the yearly subscription are discounted by 10%.<br>
          ✔ The rates are subject to change without any prior intimation.<br>
          ✔ Changes in rates shall not affect your current membership for the duration of the membership.<br>
          ✔ Renewal of Membership shall be done only on the applicable rates at the time of Renewal.<br>
          ✔ The participation fee of the successful seller shall be adjusted against his commission.<br>
          ✔ The Inaugural offer of an additional period in the same price is valid for a limited period and can be
          withdrawn at any time at the discretion of TECHOTRADE.ORG</span>
      </b-col>
      <b-col offset-lg="1" lg="5">
        <b-row class="detail-row">
          <b-col lg="5">
            <h1 class="sub-title">Membership Type</h1>
          </b-col>
          <b-col lg="6">
            <b-form-select v-model="selectedMembership" :options="options"></b-form-select>
          </b-col>
        </b-row>
        <b-row class="detail-row">
          <b-col lg="5">
            <h1 class="sub-title">Membership Amount (INR)</h1>
          </b-col>
          <b-col lg="5">
            <p class="amount" v-if="selectedMembership!=null"> {{ selectedMembership[1] }}</p>
            <p class="amount" v-else>0</p>
          </b-col>
        </b-row>
        <div class="pay-btn-div">
          <b-button variant="danger">Proceed To Pay</b-button>
        </div>
      </b-col>
    </b-row>
    <b-row>
      <b-col offset-lg="4">
      <h1 class="title2">Our Bank Details For Accounting Purpose</h1>
      <div class="bank-div">
      <span class="bank"><strong> Name of The Account</strong> : ECP COMMERCIALt Pvt. Ltd.<br>
        <strong>Account No.</strong>  : 50200011822327<br>
        <strong>Bank</strong> : HDFC Bank Limited<br>
        <strong>Branch</strong> : Gandhi Nagar RANCHI<br>
        <strong>RTGS/IFSC</strong> : HDFC0000573<br>
      </span>
      </div>

      </b-col>
    </b-row>

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
    font-size: 1.2em;
    font-weight: bold;
    margin-left: 5px;
    text-transform: uppercase;
  }

    .title2 {
    font-size: 1.2em;
    font-weight: bold;
    margin-top: 60px;
    text-transform: uppercase;
    text-align: left;
  }

  .sub-title {
    font-size: 1.1em;
    font-weight: bold;
    margin-left: 5px;
    text-transform: uppercase;
    margin-top: 10px;
    text-align: left;
  }

  .table-div {
    margin-bottom: 20px;
  }

  .offer-div {
    text-align: left;
  }

  .offer {
    font-size: 0.9em;
    font-weight: bold;
  }

  .amount {
    width: 100%;
    text-align: left;
    margin-top: 8px;
    font-weight: bold;
  }

  .pay-btn-div {
    text-align: center;
    width: 100%;
    margin-top: 20px;
  }

  .bank-div{
    text-align: left;
    width: fit-content;
  }

  .bank{
    font-size: 0.9em;
  }
</style>





<script>
  export default {
    data() {
      return {
        selectedMembership: null,
        fields: ['Plan',
          {
            label: 'Membership fee (INR)',
            key: 'Membership'
          },
          {
            label: 'Participation fee (INR)',
            key: 'Participation'
          },
          {
            label: 'Gross Transaction Value Commission',
            key: 'Gross'
          },
          {
            label: 'E-Brochure',
            key: 'Brochure'
          }, 'Microsite', 'Advertisement',
        ],
        items: [{
            Plan: "Quarter Subscription (3 Month)",
            Membership: 35400.00,
            Participation: '0',
            Gross: '1%',
            Brochure: 'Eligible',
            Advertisement: 'Eligible',
            Microsite: 'Eligible'
          },
          {
            Plan: "Half Yearly Subscription (6 Months)",
            Membership: 66080.00,
            Participation: '0',
            Gross: '1%',
            Brochure: 'Eligible',
            Advertisement: 'Eligible',
            Microsite: 'Eligible'
          },
          {
            Plan: "Yearly Subscription(1 Year+ 3 Month Free)",
            Membership: 122000.00,
            Participation: '0',
            Gross: '1%',
            Brochure: 'Eligible',
            Advertisement: 'Eligible',
            Microsite: 'Eligible'
          }
        ],
        options: [{
            value: null,
            text: ' -- Please select a Membership Type -- ',
            disabled: true
          },
          {
            value: ['Quarter', '35400'],
            text: 'Quarter Subscription'
          },
          {
            value: ['Half', '66080'],
            text: 'Half Yearly Subscription'
          },
          {
            value: ['Yearly', '122000'],
            text: 'Yearly Subscription'
          }
        ]
      }

    }
  }
</script>