<template>
  <div id="app">
    <!-- <Sidebar></Sidebar> -->
    <Map></Map>
  </div>
</template>

<script>
// import Sidebar from './components/Sidebar.vue'
import Map from './components/Map.vue'

export default {
  name: 'App',
  components: { Map }
}
</script>

<style>

@import 'https://api.mapbox.com/mapbox-gl-js/v1.10.1/mapbox-gl.css';

* {
  box-sizing: border-box;
}
#app {
  display: flex;
}

aside {
  display: none;
  width: 200px;
  background: #cecece;
  height: 100vh;  
}

.active { 
  display: block;
}

a {
    display: block;
    padding: 10px 5px;
    color: #666;
    border-bottom: 1px solid #bbb;
}

.wrapper {
  display: flex;
  align-items: stretch;
  flex-direction: column;
  width: 100vw;
}

header {
  width: 100%;
  padding: 10px;
  background: #aaa;
}

main {
  flex-grow: 2;
  padding: 10px;
}
</style>