<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12" id="createForm">
        <div id="backboard">
          <notifications group="login" />
          <div class="text-center" id="login">
            <form @submit.prevent="loginUser">
              <!-- <label for="input1">Email</label> -->
              <div class="form-group center">
                <input
                  class="form-control"
                  id="inputAddress"
                  type="text"
                  placeholder="Username"
                  required
                />
              </div>
              <!-- <label for="input2">Password</label> -->
              <div class="form-group">
                <input
                  class="form-control"
                  id="input2"
                  type="password"
                  placeholder="Password"
                  required
                />
              </div>
              <div class="form-group">
                <input class="form-control" id="input3" type="text" placeholder="Email" required />
              </div>
              <div class="form-row">
                <div class="form-group col-md-6">
                  <input
                    class="form-control"
                    id="input4"
                    type="text"
                    placeholder="First Name"
                    required
                  />
                </div>
                <div class="form-group col-md-6">
                  <input
                    class="form-control"
                    id="input5"
                    type="text"
                    placeholder="Last Name"
                    required
                  />
                </div>
              </div>
              <button type="submit">Login</button>
            </form>
          </div>
          <p>
            Don't have an account?
            <!-- <router-link to="/sign_up" tag="h6" id="sign-up">Create One</router-link> -->
          </p>
        </div>
      </div>
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
#createForm {
  display: flex;
  justify-content: center;
}
</style>