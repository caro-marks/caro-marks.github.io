<template>
  <div class="box">
    <Presentation />
    <SkillSet />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { SkillSet } from '@/components/molecules'
import { Presentation } from '@/components/organisms'
export default defineComponent({
  components: {
    Presentation,
    SkillSet
  }
})
</script>

<style lang="scss" scoped>
.box {
  width: 90%;
  max-width: 1150px;
  margin: 0 auto;
  max-height: 80vh;
}
</style>
