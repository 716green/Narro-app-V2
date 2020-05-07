<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="https://www.creative-tim.com">
              ABC
            </a>
          </li>
          <li>
            <a href="https:///presentation.creative-tim.com">
              DEF
            </a>
          </li>
          <li>
            <a href="https:///blog.creative-tim.com">
              GHI
            </a>
          </li>
          <li>
            <a href="https://www.creative-tim.com/license">
              JKL
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }} Narro, LLC
        <!-- , made with <md-icon>favorite</md-icon> by
        <a href="https://www.creative-tim.com/" target="_blank">Creative Tim</a>
        for a better web. -->
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
