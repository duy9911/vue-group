<template>
  <div class="login-form">
    <form>
      <h3>Sign In</h3>

      <div class="form-group">
        <label>Email address</label>
        <input
          type="email"
          v-model="infor.email"
          class="form-control form-control-lg"
        />
      </div>

      <div class="form-group">
        <label>Password</label>
        <input
          type="password"
          v-model="infor.password"
          class="form-control form-control-lg"
        />
      </div>

      <button type="submit" class="btn btn-dark btn-lg btn-block">
        Sign In
      </button>
    </form>
  </div>
</template>
<script>
export default {
  data() {
    return {
      infor: {
        email: "",
        password: "",
      },
    };
  },
};
</script>

<style>
* {
  box-sizing: border-box;
}

.login-form {
  width: 50%;
  margin: 20% 25%;
}
body {
  background-image: url("../assets/tea.jpg");
  min-height: 100vh;
  display: flex;
  font-weight: 400;
}
.btn{
  margin-top: 5%;
}
</style>
