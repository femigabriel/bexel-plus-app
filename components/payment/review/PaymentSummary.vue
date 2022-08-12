<template>
  <div class="summary-slip">
    <div class="summary-box">
      <div class="summary-title">
        <h3>Transfer summary</h3>
        <a href="">Edit</a>
      </div>
      <div class="summary-card">
        <p>
          <span>Send Amount</span>
          <span>
            <img src="../../../images/canada-flag.svg" alt="cad" />
            1,000 USD</span
          >
        </p>
        <p><span>Exchange rate</span><span>3.79</span></p>
        <p><span>Fees</span><span class="greentext">Free</span></p>
        <p>
          <span>Recipent gets</span
          ><span
            ><img src="../../../images/brazil-flag.svg" alt="brl" />3,900
            BRL</span
          >
        </p>
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
.summary-box {
  width: 100%;
  max-width: 727.766px;
  flex-direction: column;
  align-items: flex-start;
  padding-top: 1.5%;
  padding: 3% 4%;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
}
.summary-title {
  align-items: flex-start;
  padding-top: 1.5%;
  display: flex;
  justify-content: space-between;
  font-size: 12px;
}
.summary-title a {
  color: #1890ff;
  font-size: 12px;
}
.summary-title h3 {
  color: #4a4b65;
  font-size: 12px;
}
.summary-card {
  width: 100%;
  display: flex;
  flex-direction: column;
  padding: 20px 0;
}
.summary-card p {
  display: flex;
  justify-content: space-between;
  font-size: 14px;
  padding: 0.3rem 0;
  font-weight: 500;
}
span:first-child {
  color: #879dad;
}
span:last-child img {
  margin-right: 5px;
}
span:last-child {
  color: #4a4b65;
  display: flex;
  align-items: center;
  font-size: 14px;
  font-weight: 600;
}
.section-divider {
  display: flex;
  width: 100%;
  height: 1px;
  background-color: #b4bec6;
  opacity: 0.4;
  margin-bottom: 16px;
  margin-top: 20px;
}
</style>
