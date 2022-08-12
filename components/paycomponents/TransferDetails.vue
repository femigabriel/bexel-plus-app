<template>
  <div>
    <PaymentTransafer />
    <PaymentCalculator />
    <PaymentDeposit />
    <PaymentNext />
  </div>
</template>

<script>
import PaymentTransafer from '../payment/transfer/PaymentTransafer.vue';
import PaymentCalculator from '../payment/transfer/PaymentCalculator.vue';
import PaymentDeposit from '../payment/transfer/PaymentDeposit.vue';
import PaymentNext from '../payment/select/PaymentNext.vue';



export default {
  components: {
    PaymentTransafer,
    PaymentCalculator,
    PaymentDeposit,
    PaymentNext,
  },
};
</script>

<style></style>
