import PaymentProfileVue from './payment/PaymentProfile.vue';
<template>
  <div>
    <PaymentType />
    <PaymentProfile />
    <PaymentNext />
  </div>
</template>

<script>
import PaymentHeader from "../payment/select/PaymentHeader.vue";
import PaymentType from "../payment/select/PaymentType.vue";
import PaymentProfile from "../payment/select/PaymentProfile.vue";
import PaymentNext from "../payment/select/PaymentNext.vue";
export default {
  components: {
    PaymentHeader,
    PaymentType,
    PaymentProfile,
    PaymentNext,
  },
};
</script>

<style></style>
