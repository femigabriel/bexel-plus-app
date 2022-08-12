<template>
  <div class="level">
    <div class="page-header">
      <div class="level-title">
        <h2>Verification Levels</h2>
        <span class="badge success">50% VERIFIED</span>
      </div>
    </div>
    <div class="box-wrapper">
      <div class="box-container">
        <div class="shadow-box shadow-box-highlight">
          <div class="box-heading">
            <h3>LEVEL 1</h3>
            <i class="las la-exclamation-circle"></i>
          </div>
          <div class="subtitle"><p>$1000 Dollar Limit</p></div>
          <div class="wrap">
            <p>Personal info</p>
            <p>Phone Verification</p>
            <p class="fade-text">School information</p>
            <p>Verification</p>
          </div>
        </div>
      </div>
      <div class="box-container">
        <div class="shadow-box">
          <div class="box-heading">
            <h3>LEVEL 2</h3>
            <i class="las la-exclamation-circle"></i>
          </div>
          <div class="subtitle"><p>$2000 Dollar Limit</p></div>
          <div class="wrap">
            <p>To upgrade to this level, upload your XXXX Document Below</p>
          </div>
        </div>
        <div class="btn">
          <button>Choose File</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.level {
  /* display: flex; */
}
.level-title {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: flex-start;
  width: 100%;
  margin-bottom: 0.8rem;
}
.level-title h2 {
  font-size: 14px;
  line-height: 1.5;
  color: rgb(74, 75, 101);
}
span.badge {
  margin-left: 15px;
  height: fit-content;
}
.badge.success {
  color: rgb(18, 157, 98);
  border: 1px solid rgb(15, 197, 120);
  background: rgba(15, 197, 120, 0.2);
}
.badge {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 11px;
  font-weight: 700;
  padding: 3px 1rem;
  border-width: 1px;
  border-style: solid;
  border-radius: 6px;
}

/* box */
.box-wrapper {
  display: flex;
  flex-wrap: wrap;
  margin-top: 1.2rem;
}
.box-container {
  display: flex;
  flex-direction: column;
  width: 35%;
  margin-right: 2%;
  /* background: rgb(255, 255, 255); */
}
.shadow-box-highlight {
  background: rgb(255, 255, 255);
  border: 1px solid rgb(1, 94, 255);
  border-image: initial;
  border-radius: 6px;
}
.shadow-box {
  margin-bottom: 0.5rem;
  flex-direction: column;
  padding: 25px;
  background: rgb(255, 255, 255);
}
.box-heading {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}
.box-heading h3 {
  color: rgb(135, 157, 173);
  font-weight: 700;
  margin-bottom: 0px;
}
.box-heading img {
  position: relative;
  top: -5px;
}
.shadow-box .subtitle p {
  margin-top: 2px;
  color: rgb(1, 94, 255);
  font-size: 12px;
}
.las {
  color: rgb(1, 94, 255);
}
.shadow-box p {
  color: rgb(74, 75, 101);
  font-weight: 500;
  margin-bottom: 0px;
  display: flex;
  align-items: center;
}
.fade-text {
  color: rgb(129, 130, 153);
}
.wrap {
  margin-top: 12px;
}

/* input */
label {
  overflow: hidden;
}
#choose-file {
  display: none;
}
input {
  overflow: visible;
}
.shadow-box {
  margin-bottom: 8px;
  flex-direction: column;
  /* padding: 8%; */
}
.button {
  text-align: center;
  display: flex;
  justify-content: center;
  color: rgb(1, 94, 255);
  font-weight: 700;
  cursor: pointer;
  position: relative;
  padding: 5px 120px;
  border: 1px solid rgb(1, 94, 255);
  border-radius: 6px;
}
.btn {
  /* padding: 5px 120px; */
}
button {
  background: rgb(255, 255, 255);
  border: 1px solid rgb(1, 94, 255);
  padding: 10px 120px;
  font-size: 14px;
  color: rgb(1, 94, 255);
  border-radius: 6px;
}
</style>
