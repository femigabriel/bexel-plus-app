<template>
  <div class="hide-bar">
    <div class="aside-hide">
      <div class="logo">
        <img class="" src="../../images/bevel-logo.svg" alt="" />
      </div>
      <nav class="hide">
        <ul>
          <li class="hiden" v-for="item in items" :key="item.id">
            <NuxtLink
              :to="item.linkName"
              :class="{ active: $nuxt.$route.path == item.linkName }"
            >
              <i :class="item.icon"></i>
              {{ item.name }}</NuxtLink
            >
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default { 
  data() {
    return {
    //   isHidden: true,
      items: [
        { id: 0, name: "Dashboard", icon: "las la-home", linkName: "/" },
        {
          id: 1,
          name: "Make payment",
          icon: "las la-credit-card",
          linkName: "/payment",
        },
        {
          id: 2,
          name: "Transaction history",
          icon: "las la-hourglass-end",
          linkName: "/transactions",
        },
        {
          id: 3,
          name: "Recipents",
          icon: "las la-address-book",
          linkName: "/recipents",
        },
        {
          id: 4,
          name: "My Account",
          icon: "las la-user-alt",
          linkName: "/account",
        },
      ],
    };
  },
};
</script>

<style scoped>
.hide-bar {
  position: fixed;
  display: flex;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 100vh;
  z-index: 100;
  background: rgba(0, 0, 0, 0.226);
}
.aside-hide {
  width: 100%;
  max-width: 235px;
  padding: 20px;
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
.hide {
  margin-top: 5rem;
  width: 100%;
}
.hide ul {
  list-style: none;
  padding: 0;
  margin-top: 0;
  margin-bottom: 16px;
}
/* .active {
  color: #015eff;
  font-weight: 600;
} */
.hide ul li {
  display: flex;
  justify-content: flex-start;
  margin: 15px 10px;
  background-color: transparent;
  outline: none;
  cursor: pointer;
  transition: color 0.3s;
  text-decoration: none;
  font-size: 14px;
}
.hide li .las {
  margin-right: 10px;
  margin-bottom: 5px;
  color: #015eff;
  font-size: 18px;
}
a {
  text-decoration: none;
  color: unset;
}
</style>
