<template>
  <div>
    <input type="text" v-model="loginForm.username" placeholder="Enter email" />
    <br />
    <br />
    <input
      type="password"
      v-model="loginForm.password"
      placeholder="Enter password"
    />
    <br />
    <br />

    <button v-on:click="getLoginData">Login</button>
  </div>
</template>

<script>
export default {
  name: 'Login',

  data() {
    return {
      loginForm: {
        username: null,
        password: null,
      },
    };
  },
  methods: {
    getLoginData() {
      console.warn(this.loginForm);
    },
  },
};
</script>
