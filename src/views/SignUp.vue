<template>
  <div class="SignUp">
    <div class="container h-100">
      <form v-on:submit.prevent="submit()">
        <ul>
          <li v-for="error in errors" v-bind:key="error">{{ error }}</li>
        </ul>
        <div class="">
          <form class="form-example" action="" method="">
            <h1>Sign Up</h1>
            <!-- Input fields -->
            <div class="">
              <div class="">
                <div><label for="floatingInput">Email address</label></div>
                <input type="email" v-model="email" class="form-control" placeholder="email address" />
              </div>
            </div>
            <div class="form-group">
              <div class="">
                <div><label for="floatingInput">Password</label></div>
                <input type="password" v-model="password" class="form-control" placeholder="password" />
              </div>
            </div>
            <div class="form-group">
              <div class="">
                <div><label for="floatingInput">Password confirmation</label></div>
                <input type="password" v-model="password_confirmation" class="form-control" placeholder="password" />
              </div>
            </div>
            <!-- End input fields -->
            <button type="submit" value="Submit" class="">Sign Up</button>
          </form>
        </div>
      </form>
    </div>
  </div>
</template>

<style></style>

<script>
export default {
  data: function () {
    return {
      errors: [],
      email: "",
      password: "",
      password_confirmation: "",
    };
  },
  created: function () {},
  methods: {},
};
</script>
