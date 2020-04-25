<template>
  <div class="social-container">
    <md-list-item href="https://twitter.com/CreativeTim" target="_blank">
      <i class="fab fa-twitter"></i>
      <p class="hidden-lg">Twitter</p>
      <md-tooltip md-direction="bottom">Follow us on Twitter</md-tooltip>
    </md-list-item>
    <md-list-item href="https://www.facebook.com/CreativeTim" target="_blank">
      <i class="fab fa-facebook-square"></i>
      <p class="hidden-lg">Facebook</p>
      <md-tooltip md-direction="bottom">Like us on Facebook</md-tooltip>
    </md-list-item>
    <md-list-item
      href="https://www.instagram.com/CreativeTimOfficial"
      target="_blank"
    >
      <i class="fab fa-instagram"></i>
      <p class="hidden-lg">Instagram</p>
      <md-tooltip md-direction="bottom">Follow us on Instagram</md-tooltip>
    </md-list-item>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.social-container {
  display: flex;
}
</style>
