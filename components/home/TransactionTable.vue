<template>
  <div class="table main">
    <div class="table-header">
      <div class="table-title flex">
        <h2>Recent Transaction</h2>
        <NuxtLink to="/transactions">View All</NuxtLink>
      </div>
    </div>
    <Tab />
  </div>
</template>

<script>
import Tab from './Tab.vue';

export default {
 components: { Tab },
};
</script>

<style scoped>
.table {
  width: 100%;
  display: flex;
  flex-direction: column;
  padding: 20px;
  overflow-y: auto;
}
.main {
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 32px;
  padding-left: 40px;
}

.table-title {
  color: rgb(74, 75, 101);
  line-height: 2;
  margin-bottom: 32px;
  display: flex;
  align-items: center;
}
.table-title h2 {
  font-size: 22px;
  font-weight: 500;
}
a {
  margin-left: 1rem;
  font-size: 15px;
  font-weight: 400;
  margin-top: 3px;
  color: rgb(1, 94, 255);
}

</style>
