<template lang="html">
  <li class="track">
    <img src="" alt="" class="track__frame">
    <h3 class="track__artist"> {{ track.artist }} </h3>
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
