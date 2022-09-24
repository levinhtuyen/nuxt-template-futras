<template>
  <footer class="footer">
    <div class="footer-top section">
      <div class="container">
        <div class="footer-list">
          <p class="footer-list-title">Subscribe Newsletter</p>

          <p class="footer-list-text">
            Lorem Ipsum has been them an industry printer took a galley make
            book.
          </p>

          <form action="" class="footer-form">
            <input
              type="email"
              name="email_address"
              aria-label="email"
              placeholder="Enter email"
              required
              class="email-field"
            />

            <button type="submit" class="btn btn-secondary">
              Subscribe Now
            </button>
          </form>
        </div>

        <ul class="footer-list">
          <li>
            <p class="footer-list-title">All Courses</p>
          </li>

          <li>
            <a href="#" class="footer-link">Daily Exercise</a>
          </li>

          <li>
            <a href="#" class="footer-link">Find Your Balance</a>
          </li>

          <li>
            <a href="#" class="footer-link">Personal Program</a>
          </li>

          <li>
            <a href="#" class="footer-link">Natural Process</a>
          </li>

          <li>
            <a href="#" class="footer-link">Immune System</a>
          </li>

          <li>
            <a href="#" class="footer-link">Gives You Energy</a>
          </li>
        </ul>

        <ul class="footer-list">
          <li>
            <p class="footer-list-title">Help Links</p>
          </li>

          <li>
            <a href="#" class="footer-link">Privacy Policy</a>
          </li>

          <li>
            <a href="#" class="footer-link">Discussion</a>
          </li>

          <li>
            <a href="#" class="footer-link">Terms & Conditions</a>
          </li>

          <li>
            <a href="#" class="footer-link">Customer Support</a>
          </li>

          <li>
            <a href="#" class="footer-link">Course FAQ’s</a>
          </li>

          <li>
            <a href="#" class="footer-link">Online Classes</a>
          </li>
        </ul>

        <ul class="footer-list">
          <li>
            <p class="footer-list-title">Opening Hours</p>
          </li>

          <li>
            <a href="#" class="footer-link">Mon-Fri: 9 AM – 6 PM</a>
          </li>

          <li>
            <a href="#" class="footer-link">Saturday: 9 AM – 4 PM</a>
          </li>

          <li>
            <a href="#" class="footer-link">Sunday: Closed</a>
          </li>

          <li>
            <p class="footer-list-title address-title">Location</p>
          </li>

          <li>
            <address class="address">
              176 W street name, New<br />
              York, NY 10014
            </address>
          </li>
        </ul>
      </div>
    </div>

    <div class="footer-bottom">
      <div class="container">
        <p class="copyright">
          &copy; 2022 Futras Made With
          <LogoGithub /> by
          <a href="#" class="copyright-link">codewithsadee</a>
        </p>

        <ul class="footer-bottom-list">
          <li class="footer-bottom-item">
            <a href="#" class="footer-bottom-link">Terms of Service</a>
          </li>

          <li class="footer-bottom-item">
            <a href="#" class="footer-bottom-link">Privacy Policy</a>
          </li>

          <li class="footer-bottom-item">
            <a href="#" class="footer-bottom-link">Sitemap</a>
          </li>

          <li class="footer-bottom-item">
            <a href="#" class="footer-bottom-link">Security</a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
import LogoGithub from "vue-ionicons/dist/logo-github.vue";
export default {
  components: {
    LogoGithub,
  },
};
</script>

<style lang="scss" scoped></style>
