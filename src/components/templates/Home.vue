<template>
  <div class="box-home">
    <div class="home">
      <Header />
    </div>
    <div class="lateral">
      <Presentation />
      <Presentation />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Header, Presentation } from '@/components/organisms'

export default defineComponent({
  components: {
    Header,
    Presentation
  },
  beforeCreate() {
    console.log(window.innerHeight)
  }
})
</script>

<style lang="scss" scoped>
.box-home {
  min-height: 333px;
  max-height: 35vh;
  .lateral {
    display: flex;
    flex-direction: column;
  }
}
@media only screen and (min-width: 915px) {
  .box-home {
    .lateral {
      flex-direction: row;
    }
  }
}
</style>
