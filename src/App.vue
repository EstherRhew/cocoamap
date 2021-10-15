<template>
  <div>
    <MainLayout />

    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";

import MainLayout from "@/views/layouts/MainLayout.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    MainLayout,
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
  /* margin-top: 60px; */
}
</style>
