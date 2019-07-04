<template>
  <header class="header">
    <h1>Three simple pages</h1>
    <div id="nav">
      <router-link to="/">Main page |</router-link>
      <router-link to="/gallery">Gallery |</router-link>
      <router-link to="/about">About</router-link>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
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