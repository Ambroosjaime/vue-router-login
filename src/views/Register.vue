<template>
  <div id="register">
    <h1>Register</h1>

    <input type="text" name="username" v-model="input.username" placeholder="Username" />

    <input type="password" name="password" v-model="input.password" placeholder="Repeat Password" />

    <input type="password" name="repeatPassword" v-model="input.repeatPassword" placeholder="Password"/>

    
    <p>
      By creating an account you agree to our
      <router-link to="/terms">Terms & Privacy?</router-link>
    </p>

    <button type="submit" class="btn3">Register</button>
  </div>
</template>

<script>
export default {
  name: "Register",
  data() {
    return {
      input: {
        username: "",
        password: "",
        repeatPassword: ""
      }
    };
  }
};
</script>
<style>
#register {
  width: 500px;
  border: 1px solid #cccccc;
  background-color: #ffffff;
  margin: auto;
  margin-top: 100px;
  padding: 20px;
}

input[type="text"] {
  display: block;
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
}
input[type="password"] {
  display: block;
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
}

.btn3{
  background-color: rgb(0, 0, 46);
  color: white;
  padding: 15px 20px;
  border: none;
  cursor: pointer;
  width: 100%;
  opacity: 0.9;
}
</style>
