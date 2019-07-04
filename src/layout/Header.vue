<template>
  <header class="header">
    <h1>Three simple pages</h1>
    <div id="nav">
      <router-link to="/">Main page |</router-link>
      <router-link to="/gallery" v-bind:images="images">Gallery |</router-link>
      <router-link to="/about">About</router-link>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
      msg: String
  },
  data() {
    return {
      images: [
        {'id': 0, 'image': 'https://placekitten.com/801/800'},
        {'id': 1, 'image': 'https://placekitten.com/802/800'},
        {'id': 2, 'image': 'https://placekitten.com/803/800'},
        {'id': 3, 'image': 'https://placekitten.com/804/800'},
        {'id': 4, 'image': 'https://placekitten.com/805/800'},
        {'id': 5, 'image': 'https://placekitten.com/806/800'},
        {'id': 6, 'image': 'https://placekitten.com/807/800'},
        {'id': 7, 'image': 'https://placekitten.com/808/800'},
        {'id': 8, 'image': 'https://placekitten.com/809/800'},
        {'id': 9, 'image': 'https://placekitten.com/810/800'}
      ]
    }
  }
}
</script>

<style scoped>
  .header {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 10px;
  }

  .header a {
    color: #fff;
    padding-right: 5px;
    text-decoration: none;
  }
</style>