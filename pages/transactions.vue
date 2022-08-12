<template>
  <div class="transacts">
    <div>
      <Header />
    </div>
    <div class="history-page">
      <TransactsHeader />
      <HistoryTable />
      <TransactsHistory />
    </div>
  </div>
</template>

<script>
import Header from "../components/home/Header.vue";
import TransactsHeader from "../components/transaction/TransactsHeader.vue";
import HistoryTable from "../components/transaction/HistoryIpnut.vue";
import TransactsHistory from "../components/transaction/TransactsHistory.vue";
export default {
  components: { Header, HistoryTable, TransactsHeader, TransactsHistory },
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
  position: fixed;
}
.transacts {
  display: flex;
  justify-content: ;
}
.history-page {
  padding: 40px 80px;
  /* padding-top: 20px; */
  width: 100%;
  height: 100vh;
  overflow-y: auto;
}
</style>
