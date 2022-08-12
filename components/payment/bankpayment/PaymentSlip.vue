<template>
  <div class="section-two">
    <div class="shadow-box">
      <div id="payment-summary-card">
        <p><span>Send Amount</span><span>1,000 USD</span></p>
        <p><span>Exchange rate</span><span>3.79</span></p>
        <p><span>Fees</span><span class="greentext">Free</span></p>
        <p><span>Recipent gets</span><span>3,900 BRL</span></p>
        <div class="section-divider"></div>
        <p><span>Receiving method</span><span>Bank Deposit</span></p>
        <div class="section-divider"></div>
        <p><span>Your total</span><span>1,000 USD</span></p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.section-two {
  display: flex;
  flex-direction: column;
}
.section-two .shadow-box {
  display: flex;
  padding: 10px 15px;
  /* background: red; */
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
}
#payment-summary-card {
  width: 100%;
  display: flex;
  flex-direction: column;
  padding: 15px;
}
#payment-summary-card p {
  width: 100%;
  display: flex;
  justify-content: space-between;
  font-weight: 500;
}
p {
  margin-top: 0;
  margin-bottom: 1em;
}
span:first-child {
  color: #879dad;
}
span:last-child {
  color: #4a4b65;
  display: flex;
  align-items: center;
}
</style>
