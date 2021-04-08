<template>
  <div class="about">
    <h1>This is a map</h1>
    <div id ="map"></div>
  </div>
</template>


<style type="text/css">
#map {
  width: 400px;
  height: 400px;
}
</style>

<script>
/* global GMaps */
export default {
  created: function() {
    this.googleMap();
  },
  methods: {
    googleMap: function() {
       var map = new GMaps({
      el: '#map',
      lat: -12.043333,
      lng: -77.028333
    });
    console.log(map);
    console.log(GMaps);
    }
}
}
</script>
