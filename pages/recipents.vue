<template>
  <div class="recipents-chart">
    <div>
      <Header />
    </div>
    <div class="recipent">
      <TransactsHeader />
      <HistoryTable />
      <RecipentsHistory />
    </div>
  </div>
</template>

<script>
import Header from "../components/home/Header.vue";
import TransactsHeader from "../components/transaction/TransactsHeader.vue";
import HistoryTable from "../components/transaction/HistoryIpnut.vue";
import RecipentsHistory from "../components/recipents/RecipentsHistory.vue";
export default {
  components: { Header, TransactsHeader, HistoryTable, RecipentsHistory },
};
</script>

<style>
@import url("http://fonts.cdnfonts.com/css/mulish");
@import url("https://cdnjs.cloudflare.com/ajax/libs/line-awesome/1.3.0/line-awesome/css/line-awesome.min.css");

:after,
:before,
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: "Mulish", sans-serif;
  width: 100%;
  color: rgba(0, 0, 0, 0.85);
  line-height: 1.5715;
  background: #f5f6f9;
  overflow-y: auto;
  min-height: 100vh;
  position: fixed;
}
.recipents-chart {
  display: flex;
  /* justify-content: space-around; */
}
.recipent {
  padding: 40px 80px;
  width: 100%;
}
</style>
