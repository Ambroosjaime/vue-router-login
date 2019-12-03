<template>
  <div id="home">
    <h1>Login</h1>
    <br>
    <p>need an account?</p><router-link to="/register"><p>Create an account?</p></router-link>
    <input type="text" name="username" v-model="input.username" placeholder="Username"/>
    <input type="password" name="password" v-model="input.password" placeholder="Password"/>
    <br>
    <router-link to=""></router-link><p>forgot your password?</p>
    <br>
    <br>
    <button type="button" class="btn1" v-on:click="login()">Sign In</button>
  </div>
</template>

<script>
export default {
  name: "home",
   data() {
    return {
      input: {
        username: "",
        password: "",
      }
    };
  }
};
</script>

<style scoped>
#home {
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


i{
  display: block;
}

button a {
   text-decoration: none;
}

.btn1{
  background-color: rgb(0, 0, 46);
  color: white;
  padding: 15px 20px;
  border: none;
  cursor: pointer;
  width: 100%;
  opacity: 0.9;
}


p{
  display: inline;
}


</style>
