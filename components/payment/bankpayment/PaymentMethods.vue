<template>
  <div class="transfer">
    <div class="page-title">
      <h1>Payment</h1>
    </div>
    <div class="transfer-container"></div>
    <div class="transfer-title">
      <p>Select the payment options</p>
    </div>
    <div class="shadow-box" v-for="(box, key) in boxes" :key="key">
      <div id="custom-checkbox">
        <div class="checkbox">
          <div class="checkbox-inner"></div>
        </div>
        <div class="wrapper">
          <div class="checkbox-details">
            <p>{{ box.type }}</p>
            <p class="sub-details">
              <span> {{ box.duration }} </span>
              <span> </span>
            </p>
          </div>
          <div class="checkbox-action">
            <a class="green" href="/payment/options"> {{ box.price }} </a>
          </div>
        </div>
      </div>
    </div>
    <!-- <PaymentSlip /> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      boxes: [
        {
          type: "E-transfer",
          duration: "Transfer speed 1 hour",
          price: "free",
        },
        {
          type: "Bank payment",
          duration: "Transfer speed 1 hour",
          price: "free",
        },
        {
          type: "Debit card",
          duration: "Transfer speed 1 hour",
          price: "8.9 CAD",
        },
        {
          type: "Credit card",
          duration: "Transfer speed 1 hour",
          price: "8.9 CAD",
        },
      ],
    };
  },
};
</script>

<style scoped>
.transfer {
 
}
.transfer-container {
  width: 100%;
  padding-right: 0;
  display: flex;
  flex-direction: column;
}
.page-title h1 {
  font-size: 1.3rem;
  color: #4a4b65;
}
.page-title {
  display: flex;
  margin-bottom: 1.2rem;
  margin: 10px 0;
}
.shadow-box {
  display: flex;
  padding: 3% 4%;
  background: #ffffff;
  box-shadow: 0px 2px 5px rgba(169, 181, 192, 0.2);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
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
.inner-checkbox {
  background: #015eff;
  border-radius: 2px;
  height: 15px;
  width: 15px;
  margin: auto;
}
.wrapper {
  display: flex;
  flex-direction: row;
  align-items: center;
  flex-grow: 1;
  justify-content: space-between;
  cursor: pointer;
}
.checkbox-details {
  padding-right: 10px;
  display: flex;
  flex-direction: column;
  flex-grow: 1;
}
.checkbox-details p:first-child {
  font-weight: 600;
  font-size: 18px;
  color: #4a4b65;
  flex-grow: 1;
  margin-bottom: 0.5rem;
}
.checkbox-details p.sub-details {
  display: flex;
  justify-content: space-between;
  font-size: 14px;
  color: #879dad;
  font-weight: 400;
}
.checkbox-action {
  width: 20%;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}
a.green {
  color: #0fc578;
  font-size: 14px;
  width: 2em;
}
</style>
