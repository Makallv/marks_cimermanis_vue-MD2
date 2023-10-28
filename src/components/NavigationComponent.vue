<template>
  <div>
    <router-link to="/home" :class="{ active: isRouteActive }">Home</router-link>
    <router-link to="/about-me" :class="{ active: isRouteActive }">About Me</router-link>
  </div>
</template>

<style>
.active {
  color: blue;
}
</style>

<script>
export default {
  methods: {
    isRouteActive(route) {
      return this.$route === route;
    },
  },
};
</script>

<style scoped>
.active {
  color: #f2f2f2;
  background-color: #8645E8;
  text-decoration: none;
}
</style>