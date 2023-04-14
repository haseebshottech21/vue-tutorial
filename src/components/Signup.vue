<template>
  <div>
    <input
      type="text"
      v-model="signupForm.username"
      placeholder="Enter email"
    />

    <br />

    <br />
    <input
      type="password"
      v-model="signupForm.password"
      placeholder="Enter password"
    />

    <br />

    <p>Hobbies</p>
    <input
      type="checkbox"
      value="travel"
      v-model="signupForm.hobbies"
      id="travel"
    />
    <label for="travel">Travel</label>

    <br />

    <input
      type="checkbox"
      value="sports"
      v-model="signupForm.hobbies"
      id="sports"
    />
    <label for="sports">Sports</label>

    <br />

    <p>Gender</p>
    <input type="radio" value="male" v-model="signupForm.gender" id="male" />
    <label for="male">Male</label>

    <br />

    <input
      type="radio"
      value="female"
      v-model="signupForm.gender"
      id="female"
    />
    <label for="female">Female</label>

    <br />

    <br />

    <br />

    <button v-on:click="getSignupData">Sign Up</button>
  </div>
</template>

<script>
export default {
  name: 'Signup',

  data() {
    return {
      signupForm: {
        username: null,
        password: null,
        hobbies: [],
        gender: null,
      },
    };
  },
  methods: {
    getSignupData() {
      console.warn(this.signupForm);
    },
  },
};
</script>
