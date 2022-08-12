<template>
  <div class="main-payment">
    <div class="page-title">
      <h1>Select Recipent</h1>
    </div>
    <div class="main-title">
      <p>Choose the transaction type</p>
    </div>
    <div class="main-box">
      <div class="content-box active">
        <img src="../../../images/recipent.svg" alt="" />
        <p>To Individual</p>
      </div>
      <div class="content-box">
        <img src="../../../images/school.svg" alt="" />
        <p>To Individual</p>
      </div>
    </div>
    <div class="main-title">
      <p>Choose the transaction type</p>
    </div>
    <div class="side">
      <div class="box">
        <i class="las la-address-book"></i>
        <input type="text" placeholder="Select recipent" />
        <i class="las la-angle-down"></i>
      </div>
      <div class="side-link">
        <div>
          <p>Add new <br />recipent</p>
        </div>
        <span class="material-icons">
          <i class="las la-exclamation-circle"></i>
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.main-payment {
  /* display: flex; */
}
.page-title {
  display: flex;
  margin-bottom: 14px;
  margin: 10px 0;
}
.main-title p {
  color: #4a4b65;
  font-weight: 500;
  font-size: 14px;
  margin-top: 0;
  margin-bottom: 14px;
}
/* box */
.main-box {
  display: flex;
  grid-gap: 20px;
}
.content-box {
  max-width: 350.312px;
  width: 100%;
  display: flex;
  align-items: center;
  cursor: pointer;
  padding: 25px;
  background: #fff;
  box-shadow: 0 2px 5pxrgba (169, 181, 192, 0.2);
  border-radius: 6px;
  margin-bottom: 2rem;
}
.box {
  max-width: 455.312px;
  width: 100%;
  display: flex;
  align-items: center;
  cursor: pointer;
  padding: 25px;
  background: #fff;
  box-shadow: 0 2px 5pxrgba (169, 181, 192, 0.2);
  border-radius: 6px;
  margin-bottom: 2rem;
}
.active {
  max-width: 350.312px;
  width: 100%;
  background: linear-gradient(
    0deg,
    rgba(1, 94, 255, 0.07),
    rgba(1, 94, 255, 0.07)
  );
  border: 2px solid #015eff;
}
.content-box img {
  margin-right: 15px;
}
.content-box p {
  font-weight: 600;
  font-size: 18px;
  color: #4a4b65;
  margin-bottom: 0;
  display: flex;
}
.side {
  width: 100%;
  max-width: 755.312px;
  border-bottom: 2px solid #b4bec6;
}
input {
  height: 30px;
  border: none;
  font-size: 18px;
  width: 100%;
}
input::placeholder {
  margin: 10px;
}
.las {
  color: #9da5e1;
  font-size: 18px;
}
.las:focus {
  border: none;
}
.side-link {
  display: flex;
  margin-top: 25px;
  margin-left: 45px;
  /* width: 8em; */
}
.side-link p {
  color: #015eff;
}
.side-link .las {
  font-size: 22px;
  margin-left: 120px;
  color: #015eff;
}
.side {
  display: flex;
}
</style>
