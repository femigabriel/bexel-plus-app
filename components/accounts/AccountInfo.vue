<template>
  <div class="info">
    <div class="info-header">
      <div class="info-title"><h2>Account Settings</h2></div>
      <div class="header-title"><h4>PERSONAL INFORMATION</h4></div>
    </div>
    <div class="form-container">
      <div class="settings-box">
        <span class="icon"><i class="las la-user"></i></span
        ><input type="text" disabled="" value="Jordyn" />
      </div>
      <div class="settings-box input-item">
        <span class="icon"> <i class="las la-user"></i> </span
        ><input type="text" disabled="" value="Workman" />
      </div>
      <div class="settings-box">
        <span class="icon">
          <i class="las la-envelope"></i>
        </span>
        <input
          class=""
          type="text"
          disabled=""
          value="Jordywakman@gmail.com"
        /><button class="btn">Change</button>
      </div>
      <div class="settings-box">
        <span class="icon"> <i class="las la-envelope"></i> </span
        ><input
          class=""
          type="text"
          disabled=""
          value="+87 456 899 2345"
        /><button class="btn">Change</button>
      </div>
    </div>
    <AccountLevel />
    <AccountPassword />
  </div>
</template>

<script>
import AccountLevel from "./AccountLevel.vue";
import AccountSettings from "./AccountSettings.vue";
import AccountPassword from "./AccountPassword.vue";

export default {
  components: { AccountLevel, AccountSettings, AccountPassword },
};
</script>

<style scoped>
.info-header {
}
.info-title {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: flex-start;
  width: 100%;
  margin-bottom: 12px;
}
.info-title h2 {
  font-size: 14px;
  line-height: 1.5;
  color: #4a4b65;
  font-weight: 500;
}
.header-title {
  margin: 10px 0;
}
.header-title h4 {
  font-size: 11px;
  line-height: 14px;
  letter-spacing: 3px;
  color: #879dad;
  margin-bottom: 8px;
}
/* form */
.form-container {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.input-item {
  width: 49%;
  margin-bottom: 1.2rem;
}
.settings-box {
  display: flex;
  width: 49%;
  margin-bottom: 1.2rem;
  padding: 0.5rem 0.6rem;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
}
.las {
  color: #015eff;
}
span.icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 10%;
  height: 30px;
  margin-right: 12px;
}
#account .shadow-box input {
  border: none;
  flex-grow: 1;
}
input:disabled {
  /* all: unset; */
  border: none;
  font-weight: 500;
  font-size: 14px;
  background-color: transparent;
  color: #b4bec6;
}
.btn {
  /* all: unset; */
  background: none;
  border: none;
  margin-left: auto;
  margin-right: 0.2rem;
  color: #015eff;
  font-weight: 500;
  font-size: 14px;
}
</style>
