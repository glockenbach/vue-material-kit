<template>
  <div class="md-layout-item" ref="videoCard">
    <div class="md-card" ref="videoCard">
      <div class="md-card-media">
        <iframe
          class="md-image"
          src="data:text/html, "
          allowfullscreen
          width="0"
          height="0"
          frameborder="0"
          allowtransparency
          allow="autoplay"
          ref="videoFrame"
        ></iframe>
      </div>
      <!-- <div class="md-card-area" style="background: rgba(0, 0, 0, 0.7);">
        <div class="md-card-header">
          <span class="md-title">Solid background</span>
          <span class="md-subhead">1/1 image</span>
        </div>
      </div> -->

      <div class="md-card-content" v-show="true">
        <h5 class="card-title">{{ cardTitle }}</h5>
        <!-- <p class="card-text">
          Large | Silver | 499:-
        </p> -->

        <!-- <md-card-actions>
          <md-button>Action</md-button>
          <md-button>Action</md-button>
        </md-card-actions> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VideoCard",
  props: {
    cardTitle: {
      type: String,
      default: ""
    },
    videoSrc: {
      type: String,
      default: ""
    },
    videoRatio: {
      type: Number,
      default: 1.79
    }
  },
  data() {
    return {};
  },
  methods: {},
  mounted() {
    this.$refs.videoFrame.width = this.$refs.videoCard.clientWidth;
    this.$refs.videoFrame.height =
      this.$refs.videoCard.clientWidth / this.videoRatio;
    this.$refs.videoFrame.src = this.videoSrc;
  }
};
</script>

<style scoped lang="scss">
.md-card {
  display: inline-block;
  vertical-align: top;
}
</style>
