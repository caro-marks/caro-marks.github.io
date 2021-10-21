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
  padding: 0.5rem;
  width: 100%;
  display: grid;
  grid-template-rows: 1fr 1fr;
  align-items: center;
  .logo {
    grid-row: 2;
    padding-left: 0.1rem;
    justify-self: center;
  }
}

@media only screen and (min-width: 915px) {
  .header {
    row-gap: 0.5em;
    display: grid;
    grid-template-columns: 50% auto;
    grid-template-rows: 1fr;
    .logo {
      grid-column: 1;
      grid-row: 1;
    }
  }
}
</style>
