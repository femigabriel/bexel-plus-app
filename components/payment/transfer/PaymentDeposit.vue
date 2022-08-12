<template>
  <div class="deposit">
    <div class="deposite-title">
      <p>Choose the receiving method</p>
      <a href="">Add new</a>
    </div>
    <div class="box-container">
      <div class="deposite-box">
        <div id="custom-checkbox">
          <div class="checkbox"><div class="checkbox__inner"></div></div>
          <div class="wrapper">
            <div class="checkbox-details">
              <p>Bank Deposit</p>
              <p class="sub-details">
                <span> Zenith Bank </span> <span> Account No: 123456789 </span>
              </p>
            </div>
            <div class="checkbox-action">
              <a class="" href="/payment/transfer"> </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.deposit {
  padding-bottom: 5rem;
  display: flex;
  flex-direction: column;
  padding-right: 28%;
}
.deposite-title {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-bottom: 10px;
}
/*  */
.deposite-box {
  width: 100%;
  flex-direction: column;
  align-items: flex-start;
  padding: 3% 4%;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
}
a {
  margin-left: 10px;
  color: #015eff;
}
#custom-checkbox {
  display: flex;
  align-items: center;
  padding: 0 0.5rem;
  width: 100%;
  cursor: pointer;
}
.checkbox {
  width: 25px;
  height: 25px;
  border: 1px solid rgba(219, 221, 227, 0.7);
  box-sizing: border-box;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border-radius: 4px;
  display: flex;
  align-items: center;
  margin-right: 1.5rem;
}
#custom-checkbox .checkbox__inner {
  background: #015eff;
  border-radius: 2px;
  height: 15px;
  width: 15px;
  margin: auto;
}
</style>
