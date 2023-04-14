<template>
  <div>
    <h1>This is Data Binding Title</h1>
    <h2 style="white-space: pre-line">{{ message }}</h2>

    <!-- <input type="text" v-model="message" /> -->

    <button v-on:click="updateTitle">Update Title</button>
  </div>
</template>

<script>
export default {
  name: 'DataBind',
  methods: {
    updateTitle() {
      this.$emit('updateTitle', 'Props has been passed');
    },
  },
};
</script>
