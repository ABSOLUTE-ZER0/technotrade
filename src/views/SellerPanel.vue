<template>
  <div>
    <Header />
    <b-container fluid class="main-div">
      <b-row class="tab-row">
        <b-button @click="tab='info'" class="tab">Information</b-button>
        <b-button @click="tab='member'" class="tab">Membership Type</b-button>
        <b-button @click="tab='company'" class="tab">Company Detail</b-button>
        <b-button @click="tab='documents'" class="tab">Documents</b-button>
        <b-button @click="tab='bank'" class="tab">Bank Details</b-button>
        
      </b-row>
      <div>
        <Info v-if="tab=='info'" />
        <Membership v-if="tab=='member'" />
        <Company v-if="tab=='company'" />
      </div>

    </b-container>
  </div>
</template>

<style scoped>
.main-div{
  padding: 0 10%;
}

.tab-row{
  width: 100%;
}

.tab{
  flex: 1;
  margin: 0 10px;
}
</style>

<script>
import Header from "../components/seller/SellerHeader"
import Info from "../components/seller/Information"
import Membership from "../components/seller/Membership"
import Company from "../components/seller/Company"

export default {
  data(){
    return{
      currentTab: "Information",
      tab: "info"
    }
  },
  components:{
    Header,
    Info,
    Membership,
    Company
  }
}
</script>