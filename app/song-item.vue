<template lang="html">
  <div class="SongItem">
    <div class="panel-block">
      <div class="media is-fullwidth">
        <div class="media-left">
          <img v-bind:src="track.album.images[0].url" alt="" class="track__frame">
        </div>

        <li class="media-content track">
          <h3 class="track__artist">{{ track.artists[0].name }}</h3>
          <p class="track__name">{{ track.name }}</p>
        </li>
        <div class="media-right">
          <a v-bind:href="track.external_urls.spotify"><span class="icon is-large fa fa-spotify"></span></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['track'],
  data() {
    return {};
  },

  methods: {

  },
};
</script>
