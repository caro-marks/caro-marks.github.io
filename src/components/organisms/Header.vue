<template>
  <header class="header">
    <div class="logo">
      <HelloWorld />
    </div>
    <div class="bar">
      <NavBar />
    </div>
  </header>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { HelloWorld } from '@/components/atoms'
import { NavBar } from '@/components/molecules'

export default defineComponent({
  components: {
    HelloWorld,
    NavBar
  }
})
</script>

<style lang="scss" scoped>
.header {
  width: 100%;
  display: grid;
  grid-template-rows: 1fr 1fr;
  align-items: center;
  // justify-content: space-around;
  .logo {
    grid-row: 2;
  }
}

@media only screen and (min-width: 700px) {
  .header {
    display: grid;
    grid-template-columns: 340px auto;
    .logo {
      grid-row: 1;
    }
  }
}
</style>
