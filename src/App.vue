<template>
  <div id="app">
    <Home />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Home } from '@/components/templates'

export default defineComponent({
  components: {
    Home
  }
})
</script>

<style scoped>
#app {
  margin: 0;
  padding: 0 0.5em;
  background: #031927;
  min-height: 333px;
  max-height: 35vh;
}
</style>
