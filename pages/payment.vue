<template>
  <div class="payment-page">
    <div>
      <Header />
    </div>
    <div>
      <PaymentSidebar 
      :activeId="current"
      @setActivePage="setActivePage"
      />
      </div>

    <div class="overflow">
      <div>
        <TransactsHeader />
        <SelectRecipent v-show="current == 0" />
        <TransferDetails v-show="current == 1" />
        <MakePayment v-show="current == 2" />
        <ReviewPage v-show="current == 3" />
      </div>
    </div>
    <div class="transfer-details" v-show="current == 1"></div>
  </div>
</template>

<script>
import Header from "../components/home/Header.vue";
import PaymentSidebar from "../components/payment/select/PaymentSidebar.vue";
import SelectRecipent from "../components/paycomponents/SelectRecipent.vue";
import TransactsHeader from "../components/transaction/TransactsHeader.vue";
import TransferDetails from "../components/paycomponents/TransferDetails.vue";
import MakePayment from "../components/paycomponents/MakePayment.vue";
import ReviewPage from "../components/paycomponents/ReviewPage.vue";
export default {
  components: {
    Header,
    PaymentSidebar,
    TransactsHeader,
    SelectRecipent,
    TransferDetails,
    MakePayment,
    ReviewPage,
  },
  data() {
    return {
      current: 0,
    };
  },

  methods: {
    // nextPage() {
    //   this.current = this.current + 1;
    // },
    setActivePage(value) {
      
      this.current = value;
    },
  },
};
</script>

<style>
@import url("http://fonts.cdnfonts.com/css/mulish");
@import url("https://cdnjs.cloudflare.com/ajax/libs/line-awesome/1.3.0/line-awesome/css/line-awesome.min.css");

:after,
:before,
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: "Mulish", sans-serif;
  width: 100%;
  color: rgba(0, 0, 0, 0.85);
  line-height: 1.5715;
  background: #f5f6f9;
  position: fixed;
}
.payment-page {
  display: flex;
  width: 100%;
}
.overflow {
  padding-top: 40px;
  padding-left: 420px;
  /* padding: 80px; */
  /* flex-grow: 1; */
  display: flex;
  flex-direction: column;
  width: 100%;
  /* max-width: 1190px; */
  height: 100vh;
  overflow-y: auto;
}
.pay-flex {
  width: 100%;
  display: flex;
  padding-top: 80px;
}
.method {
  width: 100%;
  padding-right: 20px;
}
.slip {
  width: 100%;
  margin: 40px 0px;
}
.sum {
  margin-bottom: 20px;
}
</style>
