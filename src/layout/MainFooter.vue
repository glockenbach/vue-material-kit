<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
    :style="{ [`background-color`]: backgroundColor }"
  >
    <div class="container">
      <nav>
        <ul>
          <li v-show="false">
            <a href="https://www.creative-tim.com">
              Creative Tim
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, created and hosted by
        <a href="https://www.glockenbach.se/" target="_blank">Glockenbach AB</a>
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
