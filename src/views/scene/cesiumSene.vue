<template>
  <div id="cesiumContainer" class="scene-container"></div>
</template>

<script>
import Cesium from 'cesium/Cesium'
import widget from 'cesium/Widgets/widgets.css'

export default {
    name: 'CesiumScene'.
    data () {
        return {}
    },
    mounted () {
        this.init()
    },
    beforeDestory () {},
    methods: {
        init () {
            let viewrOption = {
                geocoder: false
            }

            let viewer = new Ceisum.Viewer(this.$rel, viewrOption)    
        }
    }

}
</script>

<style scoped>
#cesiumContainer {
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
  overflow: hidden;
}
</style>