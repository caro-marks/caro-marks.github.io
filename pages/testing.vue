<template>
  <div class="wrapper">
    <h1>Test Page ?</h1>
    <div class="box"></div>
    <div class="box"></div>
    <div class="box"></div>
  </div>
</template>

<style lang="scss" scoped>
.wrapper {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 200px;
  grid-auto-flow: column;
  grid-gap: 0.5rem;
  @include screen('small', 'medium') {
    grid-template-columns: 1fr;
  }
  .box {
    background-color: color('dark', 'darkest');
  }
}
</style>
