<template>
  <div class="box-home">
    <Container>
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
