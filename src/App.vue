<template>
  <div class="app">
    <router-view />
    <div id="grid">
      <div id="item1">11111111</div>
      <div id="item2">2</div>
      <div id="item3">3</div>
      <div id="item4">4</div>
      <div id="item5">5</div>
      <div id="item6">6</div>
      <div id="item6">7</div>
    </div>
  </div>
</template>
<script>
</script>
<style lang="scss" scoped>
.app {
  #grid {
    // height: 200px;
    width: 100%;
    margin: 20px;
    display: grid;
    // grid: repeat(2, 60px) / auto-flow 30px;
    // grid: auto-flow 100px / repeat(4, 1fr);
    justify-content: center;
    // grid-gap: 10px;
    justify-items: start;
    grid-template-columns: 500px 500px 150px;
    grid-template-rows: 1fr minmax(80px, 100px);
    // grid-auto-flow: row dense; /* or 'row', 'row dense', 'column dense' */
    #item1 {
      background-color: lime;
      // grid-column: span 2;
    }

    #item2 {
      background-color: yellow;
      // grid-row: span 2;
    }

    #item3 {
      background-color: blue;
      // grid-column: span 1;
    }

    #item4 {
      // grid-column-start: 2;
      background-color: red;
    }

    #item5 {
      background-color: aqua;
    }
  }
}
</style>
