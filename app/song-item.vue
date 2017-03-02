<template lang="html">
  <li class="track">
    <img src="{{ track.preview_url }}" alt="" class="track__frame">
    <h3 class="track__artist"> {{ track.artists[0].name }} </h3>
    <p class="track__name"> {{ track.name }} </p>

  </li>
</template>

<script>
export default {
  props: ['track'],
  data() {
    return {
    };
  },

  methods: {

  },
};
</script>
