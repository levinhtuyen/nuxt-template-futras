<template>
  <div>
    <!--
        - #HERO
      -->
    <section class="section hero" id="hero" >
        <div class="container">

          <p class="hero-subtitle">Fitness & Nutrition</p>

          <h1 class="h1 hero-title">This life style for your fitness, not only diet.</h1>

          <p class="hero-text">
            It has survived not only five centuries but also
          </p>

          <a href="#" class="btn btn-secondary">Start Course</a>

          <div class="social-wrapper">

            <p class="social-title">Connect with us:</p>

            <ul class="social-list">

              <li>
                <a href="#" class="social-link">
                  <LogoFacebook />
                </a>
              </li>

              <li>
                <a href="#" class="social-link">
                  <LogoGithub />
                </a>
              </li>

              <li>
                <a href="#" class="social-link">
                  <TwitterIcon />
                </a>
              </li>

              <li>
                <a href="#" class="social-link">
                  <LogoFacebook />
                </a>
              </li>

            </ul>

          </div>

        </div>
      </section>
  </div>
</template>

<script>

import LogoFacebook from "vue-ionicons/dist/logo-facebook.vue";
import TwitterIcon from "vue-ionicons/dist/logo-twitter.vue";
import LogoGithub from "vue-ionicons/dist/logo-github.vue";
  export default {
    components: {
      LogoFacebook,
      TwitterIcon,
      LogoGithub
    },

  }
</script>

<style lang="scss" scoped>

</style>
