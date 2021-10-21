<template>
  <nav class="nav-bar">
    <NavItem text="SKILLS" to="/skills" />
    <NavItem text="PROJECTS" to="/projects" />
    <NavItem text="EXPERIENCES" to="/experiences" />
    <NavItem text="ABOUT" to="/road" />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { NavItem } from '@/components/atoms'

export default defineComponent({
  components: {
    NavItem
  }
})
</script>

<style lang="scss" scoped>
.nav-bar {
  width: 100%;
  display: flex;
  justify-content: space-around;
}
// @media only screen and (min-width: 800px) {
//   .nav-bar {
//     width: 100%;
//     display: flex;
//     justify-content: space-around;
//   }
// }
</style>
