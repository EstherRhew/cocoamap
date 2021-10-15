<template>
  <div id="map" class="map"></div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "Map",
  components: {},
  mounted() {
    if (window.kakao && window.kakao.maps) {
      this.initMap();
    } else {
      const script = document.createElement("script");
      /* global kakao */
      script.onload = () => kakao.maps.load(this.initMap);
      script.src =
        "http://dapi.kakao.com/v2/maps/sdk.js?autoload=false&appkey=8c3c5d96aa047504967c27e8de71ab82";
      document.head.appendChild(script);
    }
  },
  methods: {
    initMap() {
      const container = document.getElementById("map");
      const options = {
        center: new kakao.maps.LatLng(33.450701, 126.570667),
        level: 3,
      };

      const map = new kakao.maps.Map(container, options);

      const markerPosition = new kakao.maps.LatLng(33.450701, 126.570667);
      const marker = new kakao.maps.Marker({
        position: markerPosition,
      });
      marker.setMap(map);
    },
  },
};
</script>

<style scoped>
.map {
  width: 750px;
  height: 600px;
}
</style>
