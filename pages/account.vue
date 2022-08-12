<template>
  <div class="account">
    <div>
      <Header />
    </div>
    <div class="main-page">
      <AccountHeader />
      <div class="account-page">
        <AccountSettings class="setting" />
        <AccountInfo class="info" />
        <!-- <AccountPassword /> -->
      </div>
    </div>
  </div>
</template>

<script>
import Header from "../components/home/Header.vue";
import AccountHeader from "../components/accounts/AccountHeader.vue";
import AccountSettings from "../components/accounts/AccountSettings.vue";
import AccountInfo from "../components/accounts/AccountInfo.vue";

export default {
  components: {
    Header,
    AccountHeader,
    AccountSettings,
    AccountInfo,
  },
};
</script>

<style>
:after,
:before,
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: "Mulish", sans-serif;
  width: 100%;
  color: rgba(0, 0, 0, 0.85);
  line-height: 1.5715;
  background: #f5f6f9;
  position: fixed;
}
.account {
  display: flex;
}
.main-page {
  width: 100%;
  padding: 40px 80px;
  overflow-y: auto;
  height: 100vh;
}
.account-page {
  display: flex;
  /* justify-content: space-between; */
  width: 100%;
  /* overflow-y: auto;
  height: 100vh; */
}
.setting {
  width: 100%;
  max-width: 26%;
}
.info {
  padding-top: 90px;
  padding-left: 20px;
  width: 100%;
  max-width: 74%;
}
</style>
