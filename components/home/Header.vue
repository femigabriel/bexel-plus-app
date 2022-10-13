<template>
  <section>
    <header>
      <div class="left-header flex">
        <button><i class="las la-bars"></i></button>
        <div class="logo-1">
          <img class="" src="../../images/bevel-logo.svg" alt="" />
        </div>
      </div>
      <div class="right-header flex">
        <button><i class="las la-bell"></i></button>
        <div class="avatar">
          <img src="../../images/avatar-smallsize.svg" alt="" />
        </div>
        <button class="down"><i class="las la-caret-down"></i></button>
        <button>
          <i v-on:click="isHidden = isHidden" class="las la-bars"></i>
        </button>
      </div>
      <HideBar class="aside-hide" v-show="isHidden" />
    </header>
    <!-- big size -->
    <div class="aside">
      <div class="hide-icon">
        <i v-on:click="isHidden = !isHidden" class="las la-bars"></i>
      </div>
      <div class="logo">
        <img class="" src="../../images/bevel-logo.svg" alt="" />
      </div>
      <MenuList />
    </div>
  </section>
</template>

<script>
import MenuList from "./MenuList.vue";
import HideBar from "./HideBar.vue";
export default {
  components: { MenuList, HideBar },
  data() {
    return {
      isHidden: false,
    };
  },
};
</script>

<style scoped>
.aside {
  width: 100%;
  max-width: 230px;
  padding: 25px 35px;
  box-shadow: 0 3px 5px 0 rgb(0 0 0 / 6%);
  height: 100vh;
  background-color: #fff;
  background-image: url("../../images/sidebar-shape.svg");
  background-repeat: no-repeat;
  background-position: bottom;
  background-size: contain;
  box-sizing: content-box;
  z-index: 100;
}
.sidebar {
  width: 100%;
}
header {
  display: none;
}
/* .aside {
    display: none;
  } */

.hide-icon {
  display: none;
}
.aside {
  display: none;
}
@media (max-width: 480px) {
  .aside-hide {
    display: flex;
  }
  .hide-icon {
    display: flex;
  }
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 10px;
  }
  .left-header {
    display: flex;
  }
  .right-header {
    display: flex;
    /* margin: 0 10px; */
  }
  .avatar img {
    margin: 5px 5px;
  }
  .logo-1 img {
    width: 130px;
  }
  .down .las {
    font-size: 16px;
  }
  button {
    display: flex;
    align-items: center;
    background-color: transparent;
    border: none;
    padding: 0;
    color: #4a4b65;
    font-size: 12px;
    box-shadow: none;
    margin-right: 5px;
    font-size: 24px;
    font-weight: 700;
  }
}
</style>
