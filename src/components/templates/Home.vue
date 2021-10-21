<template>
  <div class="box-home">
    <Header />
    <Presentation />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Header } from '@/components/organisms'
import { Presentation } from '@/components/organisms'

export default defineComponent({
  components: {
    Header,
    Presentation
  }
})
</script>

<style lang="scss" scoped>
.box-home {
}
@media only screen and (min-width: 915px) {
}
</style>
