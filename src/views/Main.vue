<template>
  <div class="main">
    <h1>This is main page</h1>
    <div class='main_table'>
      <div class="table_header">
        <input class="text input" placeholder="Type something...">
        <select class="select input">
          <option>Раз</option>
          <option>Два</option>
          <option>Три</option>
        </select>
        <div class="radios input">
          <label>A</label>
          <input type="radio" v-bind:value="a">
          <label>B</label>
          <input type="radio" v-bind:value="b">
          <label>C</label>
          <input type="radio" v-bind:value="c">
        </div>
      </div>
      <div class="table_menu">
      </div>
      <div class="table_content">
      </div>
    </div>
  </div>
</template>