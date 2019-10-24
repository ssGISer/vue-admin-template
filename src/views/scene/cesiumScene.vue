<template>
  <div id="cesiumContainer" />
</template>

<script>
/* eslint-disable */
import Cesium from 'cesium/Cesium'
import widget from 'cesium/Widgets/widgets.css'

export default {
  name: 'CesiumScene',
  data() {
    return {}
  },
  mounted() {
    this.init()
  },
  beforeDestory() {},
  methods: {
    init() {
      const viewrOption = {
        geocoder: false
      }
      const viewer = new Cesium.Viewer(this.$el, viewrOption)
    }
  }
}
</script>

<style scoped>
#cesiumContainer {
  width: 100%;
  height: 100%;
  overflow: hidden;
}

</style>
