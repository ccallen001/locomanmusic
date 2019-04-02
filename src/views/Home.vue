<template>
  <div class="view-home">
    <iframe
      class="reverb-nation-player"
      scrolling="no"
      frameborder="no"
      src="https://www.reverbnation.com/widget_code/html_widget/artist_3865698?widget_id=55&pwc[included_songs]=1&context_type=page_object&spoid=artist_3865698"
    ></iframe>
  </div>
</template>

<style lang="scss" scoped>
.view-home {
  .reverb-nation-player {
    display: block;
    margin: 0 auto;
    width: 300px;
    height: 390px;
  }
}
</style>


<script>
export default {
  name: "home"
};
</script>
