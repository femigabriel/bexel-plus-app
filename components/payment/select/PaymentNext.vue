<template>
  <div class="btn">
    <div class="cancel">
      <button @click="previousPage">Cancel</button>
    </div>
    <div class="next">
      <button @click="nextPage">Next</button>
    </div>
  </div>
</template>

<script>
export default {
  emits: [],
  methods: {
    previousPage() {
      this.$emit("gotoPrevious");
    },
    nextPage() {
      console.log("testo");
      this.$emit("gotoNext");
      this.current = this.current + 1;
    },
  },
};
</script>

<style scoped>
.btn {
  display: flex;
  justify-content: space-between;
  padding-top: 40px;
  padding-bottom: 80px;
  padding-right: 40px;
}
.cancel button {
  text-transform: uppercase;
  color: #818299;
  border: none;
  background-color: transparent;
  padding: 0.7rem 0;
  cursor: pointer;
}
.next button {
  background-color: #015eff;
  color: #fff;
  padding: 20px 65px;
  border-radius: 6px;
  border: none;
  cursor: pointer;
  font-size: 14px;
}
button {
  font-size: 14px;
}
</style>
