<template>
  <div class="section-two">
    <div class="section-title"><p>How much you would like to send?</p></div>
    <div class="box-container">
      <div id="currency-calculator">
        <form>
          <label
            ><div class="currency-input">
              <small>You Send</small><input type="number" placeholder="1,000" />
            </div>
            <p class="ant-dropdown-trigger currency-dropdown">
              <img src="../../../images/canada-flag.svg" alt="cad flag" />CAD
              <span class="material-icons"
                ><i class="las la-caret-down"></i
              ></span></p
          ></label>
          <div class="logic-box">
            <p>
              <span class="logic__symbols"><small>–</small></span> 20.20
              CAD<span class="logic__description">Fee (Including IOF)</span>
            </p>
            <p>
              <span class="logic__symbols"><small>=</small></span> 970.80
              CAD<span class="logic__description">Amount we'll convert</span>
            </p>
            <p>
              <span class="logic__symbols"><small>÷</small></span> 2,27361<span
                class="logic__description"
                >Commercial rate (144 hrs)</span
              >
            </p>
          </div>
          <label
            ><div class="currency-input">
              <small>They Receive</small
              ><input type="number" placeholder="3,900" />
            </div>
            <p class="ant-dropdown-trigger currency-dropdown">
              <img src="../../../images/brazil-flag.svg" alt="brl flag" />BRL
              <span class="material-icons"
                ><i class="las la-caret-down"></i
              ></span></p
          ></label>
          <!-- <div class="notice">
            <p>This page is refreshed every 60 seconds</p>
          </div>
          <div class="form__submit">
            <button class="form__submit__button">Send this Amount</button>
          </div> -->
        </form>
      </div>
      <div class="transfer-info">
        <p>
          Expected start date: <span>July 8th 2020</span>
          <span class="material-icons">
            <i class="las la-exclamation-circle"></i
          ></span>
        </p>
        <p>
          Expected completion date: <span>July 10th 2020</span>
          <span class="material-icons">
            <i class="las la-exclamation-circle"></i
          ></span>
        </p>
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
  padding-right: 28%;
}
.box-container {
  flex-direction: column;
}
.box-container {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  margin-bottom: 1.5rem;
}
#currency-calculator {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin-bottom: 1rem;
}
form {
  display: flex;
  flex-direction: column;
  width: 100%;
}
form label {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #fff;
  height: 60px;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border-radius: 6px;
  padding: 7px 10px;
  width: 100%;
}
.currency-input {
  display: flex;
  flex-direction: column;
}
.currency-input small {
  font-size: 11px;
  color: #015eff;
}
input {
  border: none;
}
.currency-dropdown {
  width: 100px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  /* margin: 0 10px; */
  border-left: 1px solid #b4bec6;
  /* height: 90%; */
}
.las {
  margin-right: 5px;

  font-size: 18px;
}
.currency-dropdown img {
  margin-right: 5px;
}
.logic-box {
  border-left-color: #015eff;
  height: 140px;
  margin-left: 35px;
  border-left: 2px dashed #fff;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}
.logic-box p {
  display: flex;
  align-items: center;
  position: relative;
  left: -11px;
  margin: 0;
  color: #4a4b65;
  font-size: 13px;
  font-weight: 500;
}
span.logic__symbols {
  background-color: #015eff;
  color: #fff;
  height: 20px;
  width: 20px;
  padding-right: 0.03rem;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 100%;
  font-weight: 700;
  margin-right: 10px;
}
.logic-box p span.logic__symbols small {
  position: relative;
  top: -1px;
  font-size: unset;
}
.logic-box p span.logic__description {
  opacity: 0.7;
  margin-left: 10px;
  font-weight: 400;
  color: #4a4b65;
}
/* transfer */
.transfer-info {
  width: 100%;
  /* border-bottom:1px solid #879dad; */
}
.transfer-info p {
  display: flex;
  width: 100%;
  justify-content: flex-start;
  align-items: center;
  color: #879dad;
}
.transfer-info p span:first-child {
  color: #4a4b65;
  margin-left: 7px;
}
 .transfer-info p span:nth-child(2) .las{
    font-size: 24px;
    margin-left: 7px;
    color: #015eff;
}
</style>
