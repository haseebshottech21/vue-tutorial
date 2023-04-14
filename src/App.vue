<template>
  <div id="app">
    <h1>{{ title }}</h1>
    <!-- <img alt="Vue logo" src="https://vuejs.org/images/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- <DataBind v-on:updateTitle="updateTitleText($event)" />
    <Child v-bind:name="name" v-bind:users="users" /> -->
    <Login />
    <br />

    <br />
    <h1>Signup Form</h1>
    <Signup />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
// import DataBind from './components/DataBind.vue';
// import Child from './components/Child.vue';
import Login from './components/Login.vue';
import Signup from './components/Signup.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // DataBind,
    // Child,
    Login,
    Signup,
  },
  data() {
    return {
      title: 'Get Form Data with Vue Js',
      name: 'Muhammad Haseeb',
      users: [
        { name: 'bruce', email: 'bruce@mail.com' },
        { name: 'jhon', email: 'jhon@mail.com' },
        { name: 'danny', email: 'danny@mail.com' },
        { name: 'bravo', email: 'bravo@mail.com' },
      ],
    };
  },
  methods: {
    updateTitleText(title) {
      this.title = title;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
