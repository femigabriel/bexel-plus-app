<template>
  <div class="trans-history">
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
          <img src="../../images/avatar-smallsize.svg" alt="" class="avatar" />
          <span class="profile-name">Femi Gabriel</span>
          <span class="icons">
            <i class="las la-caret-down"></i>
          </span>
        </button>
      </div>
    </div> 
  </div>
</template>

<script>
import TransactsHistory from './TransactsHistory.vue';
export default { components: {TransactsHistory

} };
</script>

<style scoped>
.trans-history {
  width: 100%;
  /* max-width: 1103px; */
  display: flex;
  flex-direction: column;
  width: 100%;
  /* padding: 20px 30px; */
}
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.right {
  width: fit-content;
  display: flex;
  align-items: center;
}
.notifications {
  margin: 0 5px;
}
.las {
  font-size: 28px;
}
/* .notifications span {
  position: absolute;
  right: 264px;
  top: 44px;
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
  /* color: #fff; */
  font-size: 15px;
  margin: 0 20px;
}
.avatar {
  width: 35px;
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
