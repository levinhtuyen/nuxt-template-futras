<template>
<div>
  <main>
    <article>
      <HeroVue />
      <ServiceVue />
      <AboutVue />
      <CourseVue />
      <BlogVue />
      <DownAppVue />
    </article>
  </main>
</div>
</template>

<script>
import ArrowForward from "vue-ionicons/dist/ios-arrow-forward.vue";
import TwitterIcon from "vue-ionicons/dist/logo-twitter.vue";
import MailIcon from "vue-ionicons/dist/md-mail.vue";
import LogoFacebook from "vue-ionicons/dist/logo-facebook.vue";
import LogoGithub from "vue-ionicons/dist/logo-github.vue";
import AboutVue from "../components/About.vue";
import BlogVue from "../components/Blog.vue";
import CourseVue from "../components/Course.vue";
import HeroVue from "../components/Hero.vue";
import DownAppVue from "../components/DownApp.vue";
import ServiceVue from "../components/Service.vue";
export default {
  components: {
    // LinkedinIcon,
    ArrowForward,
    TwitterIcon,
    MailIcon,
    LogoFacebook,
    LogoGithub,
    AboutVue,
    BlogVue,
    CourseVue,
    HeroVue,
    DownAppVue,
    ServiceVue
},

  data() {
    return {
      avatar: require("@/static/avatar-1.webp"),
      // ADD YOUR SOCIAL LINKS HERE 👇
      socialLinks: {
        github: "https://levinhtuyen.github.io/profile_nuxt/",
        // linkedin: "https://www.linkedin.com/in/asaoluelijah/",
        // twitter: "https://twitter.com/asaolu_elijah",
        facebook: "https://www.facebook.com/profile.php?id=100007906847424",
        mail: "levinhtuyen210@gmail.com",
        youtube: "",
      },
    };
  },

  head: {
    title: "Portfolio ⚡ - Tuyến",
    meta: [
      {
        hid: "description",
        name: "description",
        content:
          "Tuyến is an awesome front-end developer and technical writer, passionate about building solutions that works across multiple platforms with high accessibility approach. Elijah has vast knowledge in web development with over 3+ years experience in building actual products",
      },
      {
        hid: "og:title",
        name: "og:title",
        content: "Portfolio ⚡ - Tuyến",
      },
      {
        property: "og:description",
        content:
          "Tuyến is an awesome front-end developer and technical writer, passionate about building solutions that works across multiple platforms with high accessibility approach. Elijah has vast knowledge in web development with over 3+ years experience in building actual products",
      },
      {
        hid: "og:image",
        name: "og:image",
        content: require("@/static/coding.png"),
      },
    ],
  },
  methods: {
    changeAvatar() {
      if (this.avatar == require("@/static/avatar-2.webp")) {
        this.avatar = require("@/static/avatar-1.webp");
      } else {
        this.avatar = require("@/static/avatar-2.webp");
      }
    },
  },
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start();

      setTimeout(() => this.$nuxt.$loading.finish(), 500);
    });
  },
};
</script>
