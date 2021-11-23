<template>
  <div id="app">
    
    <pre-loader></pre-loader>
    
  </div>
</template>

<script>
import preloader from "./components/preloader.vue"
export default {
  components: {
    "pre-loader": preloader
  }
}
</script>

<style>

html {
  margin: 0 !important;
  padding: 0;
}

body {
  background-color: #0392BF ;
}
</style>

