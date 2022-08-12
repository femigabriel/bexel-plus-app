<template>
  <div class="mini-profile">
    <div class="circle-avatar">
      <img src="../../images/ellipse-bcg.svg" class="blue-cirlce" alt="" />
      <img src="../../images/ellipse-cover.svg" class="white-cirlce" alt="" />
      <div class="avatar-container">
        <img src="../../images/avatar-square.png" alt="" />
      </div>
    </div>
    <div class="mini-profile-details">
      <p>Femi Gabriel</p>
      <p>timfemi@gmail.com</p>
    </div>
    <div class="mini-profile-notification">
      <span class="badge success">50% VERIFICATION</span
      ><span class="material-icons">
        <i class="las la-exclamation-circle"></i>
      </span>
    </div>
    <div class="mini-profile-btn">
      <a href="/account"><button>Complete Your Profile</button></a>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style scoped>
.mini-profile {
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #0a30ba;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border-radius: 6px;
  padding: 2.5rem 2rem;
  margin-top: 40px;
}
/* avatar images */
.circle-avatar {
  display: flex;
  border-radius: 100%;
  position: relative;
  left: 25px;
}
img {
  vertical-align: middle;
  border-style: none;
}
ellipse {
  position: absolute;
  right: 0;
}
.blue-cirlce {
  position: absolute;
  right: 5px;
}
.white-cirlce {
}
.avatar-container {
  position: absolute;
  top: 0;
  left: 0px;
  right: px;
  bottom: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}
/* profile */
.mini-profile-details {
  display: flex;
  flex-direction: column;
  margin: 15px 0;
}
.mini-profile-details p:nth-child(2) {
  color: #9da5e1;
  font-size: 15px;
}
.mini-profile-details p {
  color: #fff;
  margin: 1px 0;
  text-align: center;
  font-size: 24px;
}

.mini-profile-notification {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 5px 0;
  position: relative;
}
.badge.success {
  border-color: #0fc578;
  background: rgba(15, 197, 120, 0.2);
  color: #129d62;
}
.badge {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 3px 14px;
  border: 1px solid;
  font-size: 11px;
  font-weight: 700;
  width: fit-content;
  border-radius: 6px;
}
.mini-profile-notification span:nth-child(2) {
  /* position: absolute;
  right: -45px; */
}
.material-icons {
  font-size: 24px;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  display: inline-block;
  color: #9da5e1;
  font-size: 20px;
}
.rightSidebar section .mini-profile-notification {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 5px 0;
  position: relative;
}
.mini-profile-btn {
  margin: 15px 0;
  width: 100%;
}
a {
  color: #015eff;
  text-decoration: none;
  background-color: transparent;
  outline: none;
  cursor: pointer;
  transition: color 0.3s;
}
.mini-profile-btn button {
  background: rgba(17, 22, 30, 0.2);
  border-radius: 6px;
  font-weight: 700;
  color: #fff;
  border: none;
  padding: 12px;
  width: 100%;
  font-size: 18px;
}
</style>
