import PaymentSummaryVue from '../payment/review/PaymentSummary.vue';
<template>
  <div>
    <ReviewTitle />
    <PaymentProfile />
    <PaymentSummary class="sum" />
    <ETransfer />
    <PaymentNext />
  </div>
</template>

<script>
import ReviewTitle from '../payment/review/ReviewTitle.vue';
import PaymentProfile from '../payment/select/PaymentProfile.vue';
import PaymentSummary from '../payment/review/PaymentSummary.vue';
import ETransfer from '../payment/review/ETransfer.vue';
export default {
components: {ReviewTitle, PaymentProfile, PaymentSummary, ETransfer,}
};


</script>

<style>
</style>
