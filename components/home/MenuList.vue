<template>
  <nav>
    <ul>
      <li class="" v-for="item in items" :key="item.id">
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
</template>

<script>
export default {
  data() {
    return {
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

<style>
nav {
  margin-top: 5rem;
  width: 100%;
}
ul {
  list-style: none;
  padding: 0;
  margin-top: 0;
  margin-bottom: 16px;
}
.active {
  color: #015eff;
  font-weight: 600;
}
ul li {
  display: flex;
  justify-content: flex-start;
  margin: 15px 0;
  background-color: transparent;
  outline: none;
  cursor: pointer;
  transition: color 0.3s;
  text-decoration: none;
  font-size: 14px;
}
.las {
  margin-right: 10px;
  margin-bottom: 5px;
  color: #015eff;
}
a {
  text-decoration: none;
  color: unset;
}
</style>
