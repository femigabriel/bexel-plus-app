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
        <button><i class="las la-caret-down"></i></button>
        <button><i class="las la-bars"></i></button>
      </div>
    </header>
    <!-- big size -->
    <div class="aside">
      <div class="logo">
        <img class="" src="../../images/bevel-logo.svg" alt="" />
      </div>
      <MenuList />
    </div>
  </section>
</template>

<script>
import MenuList from "./MenuList.vue";
export default {
  components: { MenuList },
};
</script>

<style scoped>.sidebar{
  width: 100%;
}
header {
  display: none;
}
.aside {
  width: 100%;
  max-width: 230px;
  padding: 25px 35px;
  box-shadow: 0 3px 5px 0 rgb(0 0 0 / 6%);
  height: 100vh;
  background-color: #fff;
  background-image: url('../../images/sidebar-shape.svg');
  background-repeat: no-repeat;
  background-position:  bottom;
  background-size: contain;
  box-sizing: content-box;
  z-index: 100;
}

@media (max-width: 480px) {
  .aside {
    display: none;
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
