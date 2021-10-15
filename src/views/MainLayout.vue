<template>
  <main>
    <ListContainer />
    <Map></Map>
  </main>
</template>

<script>
import Map from "./Map.vue";
import ListContainer from "./ListContainer.vue";

export default {
  name: "MainLayout",
  components: {
    Map,
    ListContainer,
  },
};
</script>

<style scoped>
main {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-around;
  flex: 1;
}
</style>