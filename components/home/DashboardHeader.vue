<template>
  <div class="dashboard">
    <div class="dash-title">
      <h1>DASHBOARD</h1>
    </div>
    <div class="container">
      <div class="content-title">
        <h2>Send Again</h2>
      </div>
      <div class="box-content">
        <!-- team a -->
        <div class="team-a flex">
          <div class="group-1">
            <div class="user-avatar">
              <img src="../../images/avatar-square.png" alt="" class="avatar" />
              <img src="../../images/brazil-flag.svg" alt="" class="flag" />
            </div>
          </div>
          <!--  -->
          <div class="group-2">
            <h3>Femi Gabriel</h3>
            <p>timfemi@gmail.com</p>
          </div>
        </div>
        <!-- team b -->
        <div class="team-b flex">
          <div class="group-3">
            <h3>
              <span>100 CAD</span>
              <i class="las la-caret-right"></i>
              <span>100 CAD</span>
            </h3>
            <p>Last Transaction</p>
          </div>
          <!--  -->
          <div class="group-4">
            <button>Send Money</button>
          </div>
        </div>
      </div>
    </div>
    <CreditPage />
    <TransactionTable />
  </div>
</template>

<script>
import CreditPage from "./CreditPage.vue";
import TransactionTable from "./TransactionTable.vue";
export default { components: { CreditPage, TransactionTable } };
</script>

<style scoped>
.dashboard {
  width: 100%;
  /* max-width: 920px; */
}
.dash-title h1 {
  font-size: 14px;
  color: #879dad;
  opacity: 0.5;
  padding-bottom: 10px;
}

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  padding-top: 20px;
  padding-bottom: 40px;
  padding-left: 20px;
  padding-right: 20px;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 32px;
  line-height: 22.001px;
}
.content-title {
  color: #4a4b65;
  font-size: 16px;
  line-height: 1;
  margin-bottom: 32px;
}
.box-content {
  display: flex;
  justify-content: center;
}
.user-avatar {
  display: flex;
  flex-direction: column;
}
.avatar {
  width: 75px;
}
.flag {
  width: 25px;
  margin: -15px 20px;
}
.group-2 {
  display: flex;
  flex-direction: column;
  margin: 0 20px;
}
h3 {
  margin: 0;
  display: flex;
  align-items: center;
  font-size: 16.38px;
  font-weight: 500;
  line-height: 1.5;
}
p {
  margin: 0;
  color: #879dad;
  font-size: 16px;
}
.group-1 {
  display: flex;
  flex-direction: column;
}
.group-2 {
  display: flex;
  flex-direction: column;
  width: 21em;
}
.group-3 {
  width: 22em;
}
button {
  background: #015eff;
  padding: 15px 32px;
  border: none;
  border-radius: 6px;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  font-weight: 700;
  color: #fff;
  font-size: 14px;
  width: 12em;
}

@media (max-width: 480px) {
  .dashboard {
    padding-left: 10px;
    padding-right: 20px;
  }
  .container {
    max-width: 385px;
  }
  .box-content {
    display: flex;
    flex-direction: column;
  }
  .team-a {
    display: flex;
    padding-bottom: 20px;
  }
  .team-b {
    display: flex;
  }
  .team-b h3 {
    font-size: 18px;
  }
  button {
    padding: 10px 10px;
    margin: 0px 20px;
    width: 8em;
  }
}
</style>
