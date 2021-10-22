<template>
  <div class="box-home">
    <Header />
    <SkillSet />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Header } from '@/components/organisms'
import { SkillSet } from '@/components/molecules'

export default defineComponent({
  components: {
    Header,
    SkillSet
  }
})
</script>

<style lang="scss" scoped>
.box-home {
}
@media only screen and (min-width: 915px) {
}
</style>
