<template>
  <li class="md-list-item">
    <a
      href="javascript:void(0)"
      class="md-list-item-router md-list-item-container md-button-clean dropdown"
    >
      <div class="md-list-item-content">
        <drop-down direction="down">
          <md-button
            slot="title"
            class="md-button md-button-link md-white md-simple dropdown-toggle"
            data-toggle="dropdown"
          >
            <i class="material-icons">view_carousel</i>
            <p>Examples</p>
          </md-button>
          <ul class="dropdown-menu dropdown-with-icons">
            <li>
              <router-link to="/landing">
                <i class="material-icons">view_day</i>
                <p>Landing Page</p>
              </router-link>
            </li>
            <li>
              <router-link to="/login">
                <i class="material-icons">fingerprint</i>
                <p>Login Page</p>
              </router-link>
            </li>
            <li>
              <router-link to="/profile">
                <i class="material-icons">account_circle</i>
                <p>Profile Page</p>
              </router-link>
            </li>
            <li>
              <router-link to="/components">
                <i class="material-icons">account_circle</i>
                <p>Components</p>
              </router-link>
            </li>
            <li>
              <router-link to="/">
                <i class="material-icons">layers</i>
                <p>All Components</p>
              </router-link>
            </li>
            <li>
              <a
                href="https://demos.creative-tim.com/vue-material-kit/documentation/"
              >
                <i class="material-icons">content_paste</i>
                <p>Documentation</p>
              </a>
            </li>
            <li>
              <a href="javascript:void(0)" @click="scrollToElement()">
                <i class="material-icons">cloud_download</i>
                <p>Download</p>
              </a>
            </li>
          </ul>
        </drop-down>
      </div>
    </a>
  </li>
</template>

<script>
export default {};
</script>

<style></style>
