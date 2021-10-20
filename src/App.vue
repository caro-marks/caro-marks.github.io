<template>
  <div id="app">
    <Logo />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Logo } from '@/components/atoms'
// import axios from '@/utils/axios'

export default defineComponent({
  components: {
    Logo
  }
  // data() {
  //   return {}
  // },
  // methods: {},
  // created() {}
})
</script>

<style scoped>
#app {
  width: 10%;
}
</style>
