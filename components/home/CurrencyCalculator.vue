<template>
  <div class="calculator">
    <div class="calculator-title">
      <h2>Quick Currency Converter</h2>
    </div>
    <form>
      <label
        ><div class="currency-input">
          <small>You Send</small><input type="number" placeholder="1,000" />
        </div>
        <p class="currency-dropdown">
          <img src="../../images/canada-flag.svg" alt="cad flag" />
          CAD
          <span class="currency-icons"
            ><i class="las la-caret-down"></i
          ></span></p
      ></label>
      <div class="logic-box">
        <p>
          <span class="logic-symbols"><small>–</small></span> 20.20 CAD<span
            class="logic-description"
            >Fee (Including IOF)</span
          >
        </p>
        <p>
          <span class="logic-symbols"><small>=</small></span> 970.80 CAD<span
            class="logic-description"
            >Amount we'll convert</span
          >
        </p>
        <p>
          <span class="logic-symbols"><small>÷</small></span> 2,27361<span
            class="logic-description"
            >Commercial rate (144 hrs)</span
          >
        </p>
      </div>
      <label
        ><div class="currency-input">
          <small>They Receive</small><input type="number" placeholder="3,900" />
        </div>
        <p class="currency-dropdown">
          <img src="../../images/brazil-flag.svg" alt="brl flag" />
          BRL
          <span class="currency-icons"
            ><i class="las la-caret-down"></i
          ></span></p
      ></label>
      <div class="notice"><p>This page is refreshed every 60 seconds</p></div>
      <div class="form-submit">
        <button class="submit-button">Send this Amount</button>
      </div>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style>
.calculator {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
}
.calculator h2 {
  color: #fff;
  font-size: 14px;
  text-align: left;
  width: 100%;
  padding-bottom: 6px;
}
form {
  display: flex;
  flex-direction: column;
  width: 100%;
}
label {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #fff;
  height: 70px;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border-radius: 6px;
  padding: 7px 0px;
  width: 100%;
  max-width: 30em;
}
.currency-input {
  display: flex;
  flex-direction: column;
  
}
input {
  background: rgb(255, 255, 255);
  color: rgba(0, 0, 0, 0.85);
  font-weight: 400;
  font-size: 18px;
  opacity: 0.5;
  padding-top: 5px;
}
::placeholder {
  font-size: 20px;
  padding-left: 10px;
}
.currency-input small {
  font-size: 14px;
  color: #015eff;
  padding-left: 10px;
}
.currency-icons .las {
  font-size: 18px;
  margin-top: -5px;
  margin-left: 5px;
}
.currency-input input {
  border: none;
  margin: 0;
}
.currency-dropdown {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  margin: 0;
  padding-left: 20px;
  border-left: 1px solid #b4bec6;
  height: 90%;
}
.currency-dropdown p{
  font-size: 14px;
}
.currency-icons .las{
  font-size: 18px;
}
.currency-dropdown img {
  margin-right: 5px;
}
/* login */
form .logic-box {
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
  color: #fff;
  font-size: 13px;
  font-weight: 500;
}
.logic-box p span.logic-symbols {
  height: 20px;
  width: 20px;
  padding-right: 0.03rem;
  background-color: #fff;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 100%;
  color: #015eff;
  font-weight: 700;
  margin-right: 10px;
}
span.logic-symbols small {
  position: relative;
  top: -1px;
  font-size: unset;
}
span.logic-description {
  opacity: 0.7;
  margin-left: 5px;
  font-weight: 400;
}
.notice {
  display: flex;
  justify-content: center;
  margin: 17px 0;
}
.notice p {
  margin: 0;
  text-align: center;
  color: #fff;
  opacity: 0.7;
  font-size: 14px;
}
/*  button */
.form-submit {
  display: flex;
  justify-content: center;
  align-items: center;
}
.submit-button {
  width: 100%;
  height: 60px;
  background: #0fc578;
  border: none;
  border-radius: 6px;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  font-size: 17px;
  line-height: 133.8%;
  font-weight: 700;
  color: #fff;
}
</style>
