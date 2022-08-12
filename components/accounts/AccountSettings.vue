<template>
  <div class="settings">
    <div class="settings-header">
      <div class="header-title"><h4>Transactions</h4></div>
      <div class="settings-title"><h2>My Account</h2></div>
    </div>
    <section class="container">
      <div class="settings-box active">
        <span class="icon">
          <i class="las la-cog"></i>
        </span>
        <p>Account Settings</p>
      </div>
      <div class="settings-box">
        <span class="icon">
          <i class="las la-flag"></i>
        </span>
        <p>Verification Levels</p>
      </div>
      <div class="settings-box">
        <span class="icon">
          <i class="las la-key"></i>
        </span>
        <p>Change Password</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.setting{
 
} 
.settings-header {
  margin: 10px 0;
}
.header-title {
  font-weight: 700;
  font-size: 11px;
  line-height: 14px;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: #879dad;
  margin-top: 0;
  margin-bottom: 6px;
}
.header-title {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  margin: 1.2rem 0;
}
.settings-title h2 {
  font-size: 14px;
  line-height: 133.8%;
  color: #4a4b65;
  margin: 0;
  font-weight: 500;
}
.settings-box {
  /* width: 100%; */
  max-width: 320px;
  display: flex;
  padding: 10px 15px;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
  cursor: pointer;
}
.active {
  background: linear-gradient(
      0deg,
      rgba(1, 94, 255, 0.07),
      rgba(1, 94, 255, 0.07)
    ),
    #fff;
  border: 2px solid #015eff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
}
</style>
