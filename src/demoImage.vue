<template>
  <div class="container">
    <div>
      <img src="https://picsum.photos/id/237/300/300" />
    </div>
    <div class="vertical">
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div>
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div class="big">
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div>
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div class="vertical">
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div>
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div class="horizontal">
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div>
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div class="big">
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div>
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div class="horizontal">
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div>
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div class="big">
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div>
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
    <div class="vertical">
      <img src="https://picsum.photos/id/237/100/300" />
    </div>
  </div>
</template>
<style lang="scss" scoped>
.container {
  display: grid;
  margin: 50px;
  grid-gap: 5px;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  // grid-template-rows: repeat(auto-fill, minmax(100px, 1fr));
  // grid-template: repeat(5, 50px) / repeat(2, 1fr);
  grid-auto-rows: 300px;
  grid-auto-flow: row dense;
  div {
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
  .horizontal {
    // grid-column: span 4 / 3;
    grid-column: span 2;
  }
  .vertical {
    grid-row: span 2;
  }

  .big {
    grid-column: span 2;
    grid-row: span 2;
  }
}
</style>