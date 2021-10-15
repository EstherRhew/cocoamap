<template>
  <div>
    <Header />
    <Footer />
  </div>
</template>

<script>
import Header from "@/views/layouts/Header.vue";
import Footer from "@/views/layouts/Footer.vue";

export default {
  name: "MainLayout",
  components: {
    Header,
    Footer,
  },
};
</script>

<style scoped>
</style>