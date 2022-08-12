<template>
  <div class="password">
    <div class="page-header">
      <div class="content-title"><h2>Change Password</h2></div>
      <div class="page-title">
        <h4>This will change your previous account password</h4>
      </div>
    </div>
    <div class="password-container">
      <div class="password-input">
        <span class="icon"> <i class="las la-key"></i> </span
        ><input type="text" placeholder="New password" />
      </div>
      <div class="password-input">
        <span class="icon"> <i class="las la-key"></i> </span
        ><input type="text" placeholder="Confirm new password" />
      </div>
    </div>
    <div class="btn">
      <button>Save Change</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.password {
  /* background: red; */
}
.content-title {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: flex-start;
  width: 100%;
  margin-bottom: 0.8rem;
  margin: 1.2rem 0;
}
.page-title {
  padding-bottom: 15px;
}
.page-title h2 {
  font-size: 1.2rem;
  line-height: 133.8%;
  color: #4a4b65;
}
.page-header h4 {
  font-style: normal;
  font-weight: 700;
  font-size: 11px;
  line-height: 14px;
  letter-spacing: 0.05em;
  color: #879dad;
}
/* form */
.password-container {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.input-item {
}
.password-input {
  width: 49%;
  margin-bottom: 1.2rem;
  display: flex;
  padding: 0.5rem 0.6rem;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
}
span.icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 10%;
  height: 30px;
  margin-right: 12px;
}
.las {
  /* font-size: 24px; */
  color: rgb(1, 94, 255);
}
input {
  border: none;
  flex-grow: 1;
  color: #b4bec6;
}
/* btn */
.btn {
  display: flex;

  justify-content: flex-end;
}
button {
  padding: 10px 40px;
  font-size: 14px;
  background: rgb(1, 94, 255);
  color: #fff;
  border: none;
  border-radius: 6px;
}
</style>
