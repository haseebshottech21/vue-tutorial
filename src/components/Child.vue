<template>
  <div>
    <h1>Props Component</h1>
    <h2>{{ name }}</h2>
    <div v-for="u in users" :key="user">
      <h2>{{ u.name }}</h2>
      <h2>{{ u.email }}</h2>
    </div>
    <!-- <h3>{{ users }}</h3> -->
  </div>
</template>

<script>
export default {
  name: 'Child',
  props: ['name', 'users'],
};
</script>
