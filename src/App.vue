<template>
  <div id="app">
    <Header />
    <router-view/>
  </div>
</template>

<script>
import Header from './layout/Header';
export default {
  name:"app",
  components: {
    Header
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

p {
  padding: 0 100px;
}

.main_table {
	height: 100%;
	display: grid;
	grid-template-columns: 320px 1fr;
	grid-template-rows: 60px 100%;
	grid-template-areas: "header header"  "menu content";
}

.table_header {
	width: 100%;
  grid-area: header;
}

.table_content {
	grid-area: content;
}

.table_menu {
	grid-area: menu;
	padding: 0 15px;
}

.text {
  height: 24px;
}

.select {
  height: 30px;
}

.checkbox {
  height: 30px;
  display: inline-block;
  margin: 0 10px;
}

.gallery_container {
  margin: auto auto;
  height: 50%;
  width: 50%;
}

.gallery_pic {
  height: 300px;
  width: 300px;
  margin: 5px;
}

</style>
