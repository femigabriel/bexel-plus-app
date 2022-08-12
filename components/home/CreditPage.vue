<template>
  <div class="credit">
    <div class="credit-box">
      <div class="credit-icon">
        <img src="../../images/wallet-icon-alt.svg" alt="" />
      </div>
      <div class="credit-balance">
        <p>AVAILABLE CREDIT</p>
        <h4>13,750.00 NGL</h4>
      </div>
    </div>
    <div class="credit-box">
      <div class="credit-icon">
        <img src="../../images/transaction-icon-alt.svg" alt="" />
      </div>
      <div class="credit-balance">
        <p>TOTAL TRANSACTIONS</p>
        <h4>13,750.00 NGL</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.credit {
  width: 100%;
  grid-gap: 80px;
  display: grid;
  grid-template-columns: 1fr 1fr;
}
.credit-box {
  display: flex;
  padding: 30px 40px;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
}
.credit-icon {
  background: rgba(1, 94, 255, 0.1);
  border-radius: 6px;
  padding: 0.7rem;
  margin-right: 20px;
  position: relative;
}
p {
  margin: 0;
  line-height: 133.8%;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: #818299;
  font-size: 14px;
}
h4 {
  font-size: 14.4px;
  line-height: 125%;
  letter-spacing: -0.02em;
  color: #015eff;
  margin: 5px 0;
  font-size: 14.4px;
}
@media (max-width: 480px) {
  .credit {
    width: 100%;
    grid-gap: 20px;
    display: grid;
    grid-template-columns: 1fr;
  }
}
</style>
