<template>
<div>
  <header class="header" >
    <div class="container">

      <a href="#" class="logo">
        Futras<span class="span">.</span>
      </a>

      <nav class="navbar" >

        <button class="nav-toggle-btn">
          <CloseIcon />
        </button>

        <ul class="navbar-list">

          <li class="navbar-item">
            <a href="#home" class="navbar-link">Home</a>
          </li>

          <li class="navbar-item">
            <a href="#about" class="navbar-link">About Us</a>
          </li>

          <li class="navbar-item">
            <a href="#course" class="navbar-link">All Course</a>
          </li>

          <li class="navbar-item">
            <a href="#blog" class="navbar-link">Blog</a>
          </li>

          <li class="navbar-item">
            <a href="#" class="navbar-link">Contact</a>
          </li>

        </ul>

      </nav>

      <a href="#" class="btn btn-primary">Sign Up</a>

      <button class="nav-toggle-btn" >
        <MenuIcon />
      </button>

      <div class="overlay"></div>

    </div>
  </header>
</div>
</template>

<script>
require("vue-ionicons/ionicons.css");
import SunnyIcon from "vue-ionicons/dist/md-sunny.vue";
import MoonIcon from "vue-ionicons/dist/md-moon.vue";
import CloseIcon from "vue-ionicons/dist/ios-close-circle.vue"
import MenuIcon from "vue-ionicons/dist/md-menu.vue"
export default {
  name: "NavBar",
  components: {
    SunnyIcon,
    MoonIcon,
    MenuIcon,
    CloseIcon
  },
  data() {
    return {
      themeMode: "",
    };
  },
  methods: {
    toggleDarkMode() {
      if (
        localStorage.themeMode !== undefined &&
        localStorage.themeMode != "dark"
      ) {
        localStorage.themeMode = "dark";
        document.body.classList.toggle("dark");
        document.querySelector("nav").classList.toggle("navbar-light");
        document.querySelector("nav").classList.toggle("bg-light");
        document.querySelector("nav").classList.toggle("navbar-dark");
        document.querySelector("nav").classList.toggle("bg-dark");
        this.themeMode = "dark";
      } else {
        localStorage.themeMode = "light";
        document.body.classList.toggle("dark");
        this.themeMode = "light";
        document.querySelector("nav").classList.toggle("navbar-dark");
        document.querySelector("nav").classList.toggle("bg-dark");
        document.querySelector("nav").classList.toggle("navbar-light");
        document.querySelector("nav").classList.toggle("bg-light");
      }
    },
  },
  mounted() {
    this.themeMode = localStorage.themeMode;
  },
};
</script>
<style scoped>
.navbar-nav {
  margin-left: 100px;
}
@media screen and (max-width: 420px) {
  .navbar-nav {
    margin-left: 0px;
  }
}
.nav-item {
  font-size: 14px;
  margin: 15px;
  border-radius: 2px;
}
.nav-link a {
  color: #000 !important;
  text-decoration: none;
}
.nav-item:hover {
  background: rgb(243, 240, 240);
}
.moon-icon {
  color: #000;
}
.moon-icon:hover {
  background: transparent !important;
}
.bg-light {
  background-color: #ffffff !important;
}
</style>
