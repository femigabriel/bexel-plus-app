<template>
  <div class="payment-sidebar">
    <div class="heading"><h4>Make Payment</h4></div>
    <ul>
      <li
        v-for="list in lists"
        :key="list.id"
        class="list"
        v-bind:class="{ active: list.id === activeId }"
        v-on:click="setActivePage(list.id)"
      >
        <span v-if="list.id === activeId" class="active">
          <i class="las la-check"></i>
        </span>
        <span v-else class="label">
          {{ list.numb }}
        </span>

        <span>{{ list.item }}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ["activeId"],
  data() {
    return {
      lists: [
        { id: 0, numb: 1, item: "Select recipent" },
        { id: 1, numb: 2, item: "Transfer details" },
        { id: 2, numb: 3, item: "Payment" },
        { id: 3, numb: 4, item: "Review" },
      ],
    };
  },
  emits: [],
  methods: {
    setActivePage(value) {
      // console.log(value);
      this.$emit("setActivePage", value);
      this.active = true;
    },
  },
};
</script>

<style scoped>
.payment-sidebar {
  width: 100%;
  max-width: 380px;
  padding: 4rem 35px 25px;
  height: 100vh;
  background-color: #015eff;
  color: #fff;
  position: fixed;
  z-index: 2;
  margin-bottom: 35px;
}
.heading {
  border-bottom: 1px solid #fff;
  margin-bottom: 35px;
  padding: 0.5rem 0;
}
.heading h4 {
  color: #fff;
  text-transform: uppercase;
  font-weight: 500;
  font-style: normal;
  font-size: 12px;
  line-height: 14px;
  letter-spacing: 0.05em;
}
ul {
  list-style: none;
  padding: 0;
  margin-top: 0;
  margin-bottom: 1em;
}
ul li {
  width: 100%;
  display: flex;
  align-items: center;
  font-weight: 500;
  letter-spacing: 0.05em;
  font-size: 16px;
  margin: 1.8rem 0;
  letter-spacing: 0.05em;
}
span.label {
  margin-right: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 20px;
  width: 20px;
  border: 1px solid #fff;
  border-radius: 100%;
  font-size: 12px;
  font-weight: 500;
  opacity: 0.7;
}
.active .las {
  font-size: 16px;
  color: #fff;
  background: #0fc578;
  margin: 1px 5px;
  border-radius: 50%;
}
ul li.active span {
  opacity: 1;
  color: #fff;
}
.active {
  /* opacity: 1; */
  color: red;
}
ul li span {
  opacity: 0.7;
}
</style>
