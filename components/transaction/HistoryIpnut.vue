<template>
  <div class="history">
    <div class="history-header">
      <div class="history-title">
        <h4>Transactions</h4>
      </div>
      <div class="history-content">
        <h2>Your Transactions (5)</h2>
        <form>
          <label
            ><span class="search-icons"><i class="las la-search"></i></span
            ><input type="text" placeholder="Search"
          /></label>
        </form>
      </div>
    </div>
 
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.history{
}
.history-title h4 {
  font-weight: 700;
  font-size: 11px;
  line-height: 14px;
  letter-spacing: 3px;
  color: #879dad;
  text-transform: uppercase;
  
}
.history-title {
  margin: 10px 0;
}
.history-content {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  margin: 21px 0;
}
.history-content h2 {
  font-size: ;
  line-height: 133.8%;
  color: #4a4b65;
  margin: 0;
}
form {
  width: 100%;
  max-width: 320px;
  height: 50px;
}
.search-icons .las {
  font-size: 24px;
}
input {
  border: none;
}
label {
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border-radius: 6px;
  background-color: #fff;
  display: flex;
  align-items: center;
  overflow: hidden;
  padding: 0.4rem 1.2rem;
}
</style>
