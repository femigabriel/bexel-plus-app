<template>
  <div class="right-sidebar">
    <div>
      <div class="header">
        <div class="left"></div>
        <div class="right">
          <div class="notifications">
            <div class="icon">
              <i class="las la-bell"></i>
            </div>
            <span></span>
          </div>
          <!-- not ends here -->
          <button type="button" class="btn">
            <img
              src="../../images/avatar-smallsize.svg"
              alt=""
              class="avatar"
            />
            <span class="profile-name">Femi Gabriel</span>
            <span class="icons">
              <i class="las la-caret-down"></i>
            </span>
          </button>
        </div>
      </div>
      <CurrencyCalculator />
      <CurrencyProfile />
    </div>
  </div>
</template>

<script>
import CurrencyCalculator from "./CurrencyCalculator.vue";
import CurrencyProfile from "./CurrencyProfile.vue";
export default { components: { CurrencyCalculator, CurrencyProfile } };
</script>

<style scoped>
.right-sidebar {
  height: 100vh;
  width: 100%;

  display: flex;
  flex-direction: column;
  overflow-y: auto;
  padding-top: 20px;
  padding-left: 40px;
  padding-right: 40px;
  background: linear-gradient(168.01deg, rgb(1, 133, 255), rgb(11, 7, 214));
}
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #fff;
  padding-bottom: 40px;
}
.left {
}
.right {
  width: fit-content;
  display: flex;
  align-items: center;
}
.notifications {
  margin: 0 5px;
}
.btn img {
  width: auto;
}
.las {
  font-size: 28px;
}
/* .notifications span {
  position: absolute;
  right: 0px;
  left: 0px;
  top: 20px;
  width: 8px;
  height: 8px;
  border-radius: 100%;
  background-color: #f34335;
} */
button {
  display: flex;
  align-items: center;
  background-color: transparent;
  border: none;
  padding: 0;
  color: #fff;
  font-size: 15px;
}
.avatar {
  margin: 0 5px;
}
.btn > span {
  display: inline-block;
}
@media (max-width: 480px) {
  .right-sidebar {
    display: none;
  }
}
</style>
