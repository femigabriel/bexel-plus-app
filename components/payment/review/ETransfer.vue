<template>
  <div class="e-transfer">
    <div class="box-container">
      <div class="shadow-box">
        <div class="action"><a href="/payment/review">Edit</a></div>
        <div class="box__title"><h3>E-Transfer</h3></div>
        <div id="payment-summary-card">
          <p><span>Bank:</span><span>Access (Diamond Bank)</span></p>
          <p><span>Account Name:</span><span>Bevel Plexus Texnologies</span></p>
          <p>
            <span>Account Number:</span
            ><span class="greentext">0110214749</span>
          </p>
          <p><span>Deposit Reference:</span><span>CodeQDX6MN3VSQL</span></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.e-transfer {
  display: flex;
  flex-direction: column;
  padding-right: 28%;
}
.box-container {
  margin-bottom: 0;
  display: flex;
  justify-content: space-between;
}
.shadow-box {
  display: flex;
  width: 100%;
  flex-direction: column;
  align-items: flex-start;
  padding-top: 1.5%;
  padding: 3% 4%;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
}
.action {
  display: flex;
  justify-content: flex-end;
  width: 100%;
}
.action a {
  font-size: 14px;
  color: #015eff;
}
.box__title {
  position: relative;
  top: -12px;
}
.box__title h3 {
  color: #4a4b65;
  font-size: 1rem;
}
p span:first-child {
  margin-right: 15px;
  color: #879dad;
}
span:last-child {
  color: #4a4b65;
  display: flex;
  align-items: center;
}
#payment-summary-card p {
  display: flex;
  font-weight: 600;
  font-size: 14px;
  justify-content: flex-start;
  padding: 0.4rem 0;
}
.greentext {
  color: #0fc578 !important;
}
</style>
