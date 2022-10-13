<template>
  <div class="profile">
    <div class="section-title">
      <p>Profile Recipent</p>
    </div>
    <div class="profile-box">
      <div class="action"><a href="/">Edit</a></div>

      <div class="user-info">
        <div class="team-a flex">
          <div class="group-1">
            <div class="user-avatar">
              <img src="../../../images/avatar-square.png" alt="" class="avatar" />
              <img src="../../../images/brazil-flag.svg" alt="" class="flag" />
            </div>
          </div>
          <!--  -->
          <div class="group-2">
            <h3>Femi Gabriel</h3>
            <p>timfemi@gmail.com</p>
          </div>
        </div>
        <div class="group-3">
          <h3>
            <i class="las la-mobile-alt"></i>
            <span>+1 610 435 6354</span>
          </h3>
        </div>
        <div class="group-3">
          <h3>
            <i class="las la-globe"></i>
            <span>Canada</span>
          </h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.profile {
  /* display: flex;
  justify-content: space-between; */
  padding-top: 40px;
}
.profile-box {
  max-width: 727.766px;
  width: 100%;
  flex-direction: column;
  align-items: flex-start;
  padding-top: 1.5%;
  display: flex;
  padding: 3% 4%;
  background: #fff;
  box-shadow: 0 2px 5px rgb(169 181 192 / 20%);
  border: 2px solid transparent;
  border-radius: 6px;
  margin-bottom: 2rem;
}
.action {
  display: flex;
  justify-content: flex-end;
  width: 100%;
}
.action a {
  font-size: 14px;
  color: #015eff;
  transition: color 0.3s;
}
.section-title p {
  color: #4a4b65;
  font-weight: 500;
  margin-top: 0;
  margin-bottom: 1em;
}
.user-info {
  display: flex;
  flex-direction: column;
}
.user-avatar {
  display: flex;
  flex-direction: column;
}

.user-avatar img{
  width: 75px;
}
.flag {
  width: 25px;
  margin: -15px 20px;
}
.group-2 {
  display: flex;
  flex-direction: column;
  margin: 15px 5px;
}
h3 {
  margin: 0;
  display: flex;
  align-items: center;
  font-size: 20.38px;
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

.group-3 {
  /* padding: 1px; */
  margin: 10px 0px;
}
.las {
  font-size: 26px;
}
</style>
