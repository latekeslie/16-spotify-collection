<template lang="html">
  <div class="panel section">
    <div class="panel-heading">Heeeey</div>
    <ul class="results">
      <song-item v-for="item in tracks" v-bind:track="item"></song-item>
    </ul>
  </div>
</template>

<script>
import SongItem from './song-item.vue';
export default {
  components: {
    SongItem,
  },
  created() {
    fetch(`https://api.spotify.com/v1/search?query=katy&type=track&offset=0&limit=20`)
      .then(r => r.json())
      .then((data) => {
        this.tracks = data.tracks.items
        console.log(this.tracks)
      });
  },

  data() {
    return {
      tracks: []
    };
  },

  methods: {

  },
};
</script>
