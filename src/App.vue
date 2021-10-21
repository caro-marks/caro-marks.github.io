<template>
  <div id="app">
    <Header />
    <Presentation />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Header, Presentation } from '@/components/organisms'

export default defineComponent({
  components: {
    Header,
    Presentation
  }
})
</script>

<style scoped>
#app {
  margin: 0;
  padding: 0 0.5em;
  background: #27d1b4;
  height: 50vh;
}
</style>
