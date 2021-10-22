<template>
  <div class="box">
    <slot />
  </div>
</template>

<style lang="scss" scoped>
.box {
  margin: 0 auto;
  padding: 0 0.5em;
  background: #031927;
  min-height: 333px;
  max-height: 35vh;
  width: 90%;
  max-width: 1150px;
}
</style>
