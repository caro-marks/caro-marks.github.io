<template>
  <div id="app">
    <Container>
      <Home />
    </Container>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Container } from '@/components/bosons'
import { Home } from '@/components/templates'

export default defineComponent({
  components: {
    Container,
    Home
  }
})
</script>

<style scoped>
#app {
  margin: 0;
  padding: 0 0.5em;
  background: #031927;
}
</style>
