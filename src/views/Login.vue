<template>
  <div id="backboard">
    <notifications group="login" />
    <div id="login">
      <form @submit.prevent="loginUser">
        <label for="input1">Email</label>
        <input id="input1" type="text" v-model="creds.email" required />
        <label for="input2">Password</label>
        <input id="input2" type="password" v-model="creds.password" required />
        <button type="submit">Login</button>
      </form>
      <p>
        Don't have an account?
        <!-- <router-link to="/sign_up" tag="h6" id="sign-up">Create One</router-link> -->
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Login",
  data() {
    return {
      creds: {
        email: "",
        password: ""
      }
    };
  },
  components: {}
};
</script>

<style>
</style>