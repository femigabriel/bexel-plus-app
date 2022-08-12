<template>
  <div class="transfer">
    <div class="page-title">
      <h1>Transfer Details</h1>
    </div>
    <div class="section-one">
      <div class="section-title">
        <p>When you want they receive?</p>
      </div>
      <div class="transfer-container">
        <div class="transfer-box">
          <i class="las la-calendar-minus"></i>
          <p class="flexible-text">1-2 Business Day<span>Free</span></p>
        </div>
        <div class="transfer-box">
          <i class="las la-hourglass-end"></i>
          <p class="flexible-text">Same day<span>1% of transaction</span></p>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
export default {};
</script>

<style>
.page-title {
  display: flex;
  margin-bottom: 1.2rem;
}
.page-title {
  margin: 10px 0;
}
.page-title h1 {
  font-size: 14px;
  color: #4a4b65;
}
/*  */
.section-one {
  display: flex;
  flex-direction: column;
  padding-right: 28%;
}
.section-title p {
  color: #4a4b65;
  font-weight: 500;
  margin-bottom: 1em;
}
.transfer-container {
  display: flex;
  justify-content: space-between;
}
.transfer-box {
  width: 48%;
  display: flex;
  align-items: center;
  cursor: pointer;
}
.transfer-box {
  display: flex;
  padding: 3% 4%;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
}
p.flexible-text {
  font-weight: 600;
  font-size: 18px;
  color: #4a4b65;
  display: flex;
  flex-direction: column;
}
p.flexible-text span {
  color: #879dad;
  font-size: 14px;
  font-weight: 400;
}
.transfer-box .las {
  color: #015eff;
  font-size: 42px;
}
</style>
