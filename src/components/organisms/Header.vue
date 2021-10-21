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
  padding: 0.5rem 0;
  width: 100%;
  display: grid;
  grid-template-rows: 1fr 1fr;
  align-items: center;
  .logo {
    grid-row: 2;
    justify-self: center;
  }
}

@media only screen and (min-width: 700px) {
  .header {
    row-gap: 0.5em;
    display: grid;
    grid-template-columns: 340px auto;
    grid-template-rows: 1fr;
    .logo {
      grid-column: 1;
      grid-row: 1;
    }
  }
}
</style>
