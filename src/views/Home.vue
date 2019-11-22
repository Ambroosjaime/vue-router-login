<template>
  <div class="home">
  <h1>Create a account and sign in</h1>
  <br>
  <button type="button" v-on:click="register()">Register</button>
  <h1>If you all ready have an account, please login </h1>
  <button type="button" v-on:click="login()">Login</button>
  </div>
</template>

<script>
export default {
  name: "home"
};
</script>
