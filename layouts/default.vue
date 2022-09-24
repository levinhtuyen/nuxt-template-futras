<template>
  <body>

    <NavBar />
    <div id="app">
      <Nuxt />
    </div>
    <Footer />
      <!--
        - #BACK TO TOP
      -->

    <a href="#top" class="back-top-btn" aria-label="back to top" data-back-top-btn>
      <ChevronUp />
    </a>
  </body>
</template>
<script>
  import ChevronUp from 'vue-ionicons/dist/md-arrow-down.vue'
  export default {
  components: {
    ChevronUp
  }
}
</script>
<style scoped>
#app {
  /* margin-top: 100px; */
}
</style>
