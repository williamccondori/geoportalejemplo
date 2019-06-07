<template lang="html">
    <section>
        <div id="mapid" style="width:100%;height:500px;"></div>
    </section>
</template>

<script>
export default {
  mounted() {
    var app = L.map("mapid", {}).setView([51.505, -0.09], 4);
    L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
      maxZoom: 19
    }).addTo(app);
    var basemaps = {
      PERUSAT: L.tileLayer.wms("http://localhost:8080/geoserver/UNAT/wms?", {
        layers: "UNAT:IMG_PER1_20170414151423_ORT_MS_007457",
        format: "image/png"
      })
    };
    L.control.layers(basemaps).addTo(app);
  }
};
</script>

<style scoped>
</style>