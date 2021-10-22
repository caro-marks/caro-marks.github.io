<template>
  <div class>
    <Container class="home-template">
      <Header />
      <Presentation />
    </Container>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Container } from '@/components/bosons'
import { Header } from '@/components/organisms'
import { Presentation } from '@/components/organisms'

export default defineComponent({
  components: {
    Container,
    Header,
    Presentation
  }
})
</script>
<style lang="scss" scoped>
.home-template {
  margin: 5rem auto;
  display: grid;
  grid-auto-columns: auto;
}
</style>
