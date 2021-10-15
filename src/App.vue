<template>
  <div class="app">
    <Header />
    <MainLayout />
    <Footer />
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Header from "./views/Header.vue";
import MainLayout from "./views/MainLayout.vue";
import Footer from "./views/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    MainLayout,
    Footer,
  },
};
</script>

<style>
.app {
  width: 100%;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
