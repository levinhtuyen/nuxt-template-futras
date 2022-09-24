<template>
  <div>
    <NavBar />
    <div id="app">
      <Nuxt />
    </div>
    <Footer />
      <!--
        - #BACK TO TOP
      -->

  <a href="#top" class="back-top-btn" aria-label="back to top" data-back-top-btn>
    <ion-icon name="chevron-up" aria-hidden="true"></ion-icon>
  </a>
  </div>
</template>
<style scoped>
#app {
  margin-top: 100px;
}
</style>
