/* eslint-disable */ 

<template>
  <div class="gallery">
    <h1>This is a gallery</h1>
    <div class='gallery_container'>
      <img class='gallery_pic' v-for="(image, index) in images" v-bind:key="index" :src="image.image">
    </div>
  </div>
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