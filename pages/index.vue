<template>
  <div class="app">
    <div class="side-bar">
      <Header />
    </div>
    <div>
      <div class="dash">
        <DashboardHeader class="dashboard" />
      </div>
    </div>
    <div class="right">
      <RightSidebar />
    </div>
  </div>
</template>
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
.app {
  overflow-x: hidden;
  display: flex;
}

.flex {
  display: flex;
}
.right {
  width: 100%;
}

.dash {
  padding-top: 60px;
  padding-left: 80px;
  padding-right: 20px;
  width: 100%;
  max-width: 759px;
  overflow-y: auto;
  height: 100vh;
}
/* img {
    max-width: 100%;
} */
@media (max-width: 480px) {
  .app {
    overflow-x: hidden;
    display: flex;
    flex-direction: column;
  }

  .dash {
    display: flex;
    flex-direction: column;
    padding-top: 20px;
    padding-left: 10px;
    /* margin: 10px 0px; */
    width: 100%;
  }
  .right {
    /* display: none; */
  }
}
</style>
<script>
import Header from "../components/home/Header";
import RightSidebar from "../components/home/RightSidebar.vue";
import DashboardHeader from "../components/home/DashboardHeader.vue";
export default {
  components: {
    Header,
    RightSidebar,
    DashboardHeader,
  },
  name: "IndexPage",
  data() {
    return {
      active: 0,
    };
  },
};
</script>
