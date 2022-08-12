<template>
  <div class="recipent">
    <!-- <PaymentType />
    <PaymentProfile /> -->
  </div>
</template>

<script>
import PaymentType from "../select/PaymentType.vue";
import PaymentProfile from "../select/PaymentProfile.vue";

export default { components: { PaymentType, PaymentProfile } };
</script>

<style scoped>
.recipent {
  /* display: flex;
  flex-direction: column; */
  width: 100%;
  padding: 20px 30px;
  margin-left: 410px;
  height: 100vh;
  overflow-y: auto;
}
.header {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.right {
  width: fit-content;
  display: flex;
  align-items: center;
  margin: 0 30px;
}
.notifications {
  margin: 0 5px;
}
.las {
  font-size: 28px;
}
/* .notifications span {
  position: absolute;
  left: px;
  right: px;
  top: 20px;
  width: 8px;
  height: 8px;
  border-radius: 100%;
  background-color: #f34335;
} */
button {
  display: flex;
  align-items: center;
  border: none;
  color: #4a4b65;
  font-size: 12px;
  font-weight: 500;
}
.btn {
  line-height: 1.5715;
  position: relative;
  display: inline-block;
  font-weight: 400;
  text-align: center;
  height: 32px;
  background: transparent;
}
.avatar {
  margin: 0 5px;
}
.icons .las {
  font-size: 18px;
}
.btn > span {
  display: inline-block;
}
.profile-name {
}
@media (max-width: 480px) {
  .right-sidebar {
    display: none;
  }
}
</style>
